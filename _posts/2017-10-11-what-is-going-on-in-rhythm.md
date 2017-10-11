---
layout: post
published: true
title: What is going on in Rhythm?
---
## What is going on in Rhythm?

![Signage Construction Sign.jpg]({{site.baseurl}}/img/Signage Construction Sign.jpg)


I wanted to go ahead and take a moment to write a post updating everyone on the status of my Dynamo package Rhythm.

The reason for this is because I have been doing quite a bit of work which has resulted in a few questions. Notably, my good friend [Carl Storms](https://thebimsider.com/) was prepping for a presentation and realized I removed some nodes he was using. Not exactly the most fun experience! (Sorry Carl)

Since the beginning of the year, I have had a goal of learning C# to enhance my Dynamo and Revit programming journey. This all started with a nights and weekends boot camp, which was really fun. This forced me into visual studio and expanded my thinking. During this time, I met up with my other buddy, [Marcello](http://simplycomplex.org/). He offered to show me some of the nodes he was building with C# for his custom Dynamo package simplex.

All of this led to the release of [Beaker](https://evolvelabinc.github.io/BeakerForDynamo/). Which is completely coded in C# and offers some fun stuff for Dynamo. While building [Beaker](https://evolvelabinc.github.io/BeakerForDynamo/), I realized that I appreciated the fluidity and scalability of making nodes in this way.

This caused me to want to take a second look at Rhythm. Initially, when I started the Dynamo package, I used OOTB nodes in clever ways. Along the way, I added python nodes and the count quickly rose. Within this, I had some useful nodes for setting and getting parameters.
![2017-10-11 08_32_49-Dynamo.png]({{site.baseurl}}/img/2017-10-11 08_32_49-Dynamo.png)

The problem with the methods I originally used is, to put it bluntly, they are slow. Like really slow. Which is not very fun either. Converting this stuff to C# results in huge speed upgrades.

Currently, I have migrated most of Rhythm to this new type of nodes and will push an update later next week. That means, that if you have a presentation coming up, download the latest and let me know if you have any questions. The speed increase is worth it I promise!

As always, reach out to me if you need anything! @60secondrevit, sixtysecondrevit@gmail.com

-johnP



