---
layout: post
published: false
title: 'Get #Revit Crop Region Element with #DynamoBIM'
---
A little while back I posted this clever little trick to obtain the crop region element from a section view.

http://sixtysecondrevit.com/2017-01-09-get-revit-views-section-box-with/

Essentially it is normally "-1" of the view's ElementID, but not always! Well, luckily I have been getting more into creating C# nodes for Dynamo and there are some pretty fun options within.

After reviewing a post from the very awesome [Jeremy Tammik](http://thebuildingcoder.typepad.com/blog/2013/09/rotating-a-plan-view.html) , I was able to make the following node.

![20170605-cropRegionElement.gif]({{site.baseurl}}/img/20170605-cropRegionElement.gif)

Essentially what the node does is, 

1. Disable the crop region.
2. Collect all visible elements.
3. Enable crop region.
4. Remove the previous stuff from a new collection, leaving the crop region. :)

This will be in the next Rhythm update, along with a lot of other useful ZeroTouch nodes!

Have Fun! 
-johnP