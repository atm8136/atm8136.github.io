---
layout: post
published: false
title: Rhythm Updates
---
## Rhythm Updates

Hi everyone,

I wanted to take a moment and announce some updates for Rhythm

First of all, there is a change in the library organization. Previously nodes in Rhythm that were made in C# appeared under a bin called "RevitElements". I did not like that at all, so after some help from some friends* in the community, this has been fixed.

Now Rhythm is categorized in a manner more consistent with Dynamo OOTB.
![2018-02-19_13-54-58.png]({{site.baseurl}}/img/2018-02-19_13-54-58.png)

This change caused the addition of a few new files.

![2018-02-19_13-56-31.png]({{site.baseurl}}/img/2018-02-19_13-56-31.png)
RhythmMigrations.xml is a file that should fix any unresolved errors that might happen due to the changes.
Rhythm_DynamoCustomization.xml is what makes the organization clean and pretty.

That being said, if you run into any "unresolved" or red nodes, you simply need to replace it with the new counterpart.

In addition to these core changes, I have added some new nodes and retired a few that were broken. (See the image below)
![2018-02-19_14-06-31.png]({{site.baseurl}}/img/2018-02-19_14-06-31.png)

In other news, Jason and I have launched a new MEP-centric Dynamo package called [DuctTape](https://j0hnp.bitbucket.io/ducttape/). I want to thank [Carl Storms](https://thebimsider.com/) for announcing this for us through [Twitter](https://twitter.com/theBIMsider/status/962877361090785280), nothing gets past this guy. :smiley: We will have more details on this soon.

And to round out this post, I wanted to mention my new position. Some of you may know this, but I am now a Design Technology Specialist for Parallax. This is exciting because I will be even more engaged in Dynamo development and application development in this role. Be sure to follow Parallax on [twitter](https://twitter.com/PrlxTeam), [LinkedIn](https://www.linkedin.com/company/27245331/) and check out the [website](http://www.parallaxteam.com/) as well!


-johnP

*the friends I mentioned that helped me out are [Adam](https://twitter.com/Gytaco) (audited my code), [Arthur](https://twitter.com/synthArch) (guidance on migration), and [Konrad](https://twitter.com/arch_laboratory) (generously provides his code as reference).



