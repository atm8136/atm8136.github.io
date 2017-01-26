---
layout: post
tags:
  - 'revit, rhythm, dynamo, python'
published: true
title: 'Load #Revit Views from File with #DynamoBIM'
bigimg: /img/20170125-copyFromDocument.png
---
A [question](https://forum.dynamobim.com/t/insert-from-file-views/9106/4) came up regarding loading views from files with Dynamo. A while back I added some nodes to Rhythm that do this workflow perfectly!
As you can see below we:

1.Open the source document in memory, but non visible to user.

2.Get the views, (element types).

3.And finally copy into the open document.


![graph](/img/20170125-copyFromDocument.png "Graph")


Also, here's an animation of it in action!
![gif](/img/20170125-copyViewsFromDocument.gif "Action")

<s>**Edit: after some investigation, it was discovered that this simply copies the view types for now, stay tuned for a new solution.**</s>
**Edit: I am proud to say hat this workflow can now copy the elements as well! See animation below of this new workflow.**

*First I illustrate the views and elements in the host file, then I close it out **completely**. 
*Next, I create a new file to show the loading process.

![better workflow](/img/20170126-copyViewPlusElementsFromFile.gif "Better Workflow")

Have fun!
-johnP

**Need a custom solution or workflow? [Contact us](http://www.evolvebim.com/contact) at [EvolveLAB](http://www.evolvebim.com/)! We love to do this stuff!**
