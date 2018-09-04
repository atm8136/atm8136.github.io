---
layout: post
published: true
title: 'Get the Real Display String Value of #Revit Dimensions'
date: '2018-09-04'
---
Over the long holiday weekend, an interesting discussion came up over on Twitter.
[https://twitter.com/Twiceroadsfool/status/1035656868084035584]()

Aaron has some serious model audit graphs and one of the next steps is to compare a dimension's displayed string value to what it could (or should) be if it were not rounded.

Well, thankfully the Revit API has a method that _**seems**_ to work for this. This is the ability to obtain the "ValueString" from the dimension.

[https://apidocs.co/apps/revit/2018.2/8608426e-2490-158c-f52b-f79d88f793f6.htm]()

This method has actually been exposed in Rhythm for quite some time now. 

![20180904-01.jpg]({{site.baseurl}}/img/20180904-01.jpg)

Earlier I said that is _**seems**_ to work. That is because this method always returns the dimension's string value per the project setting. 😒 (in the case of our example our project is 1/256" and the dimension type for this is 1/8")

![The string value obtained via Revit Lookup.]({{site.baseurl}}/img/20180904-02.jpg)
_The string value obtained via Revit Lookup._


After investigating this a bit through the Revit Lookup tool from [the building coder](http://thebuildingcoder.typepad.com/) , I decided to test out what would happen if we modify the project settings to match the dimension type, then retrieve the value string.

![20180904-03.jpg]({{site.baseurl}}/img/20180904-03.jpg)
_The dimension string value being reported as what we see!_

Seeing that this worked, I was very excited. We now have the logic involved that we need to roll into a solution. Here are the steps that we need to reproduce in code.

1. Get dimension's formatting given a selection.
2. Use that formatting to modify our project settings.
3. Retrieve the value string from the dimension.
4. Change the project units back to what they were.

Luckily, we are able to replicate this using a process called [Transaction Rollback](http://thebuildingcoder.typepad.com/blog/2015/02/using-transaction-groups.html). Essentially we make the changes, get the data we want and undo those changes.

Now that we have that all mapped out there will be a new node in the next release of Rhythm to do this for you. Here is a GIF of it in action.
![20180904-realDisplayString.gif]({{site.baseurl}}/img/20180904-realDisplayString.gif)

I hope this node helps people out with their model auditing tasks! (look for the next release soon)




