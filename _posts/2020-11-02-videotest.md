---
layout: post
title: 视频测试
date: 2020-11-02
Author: 七弦
tags: Test Youtube
---

测试插入youtube视频。

方法一在Youtube视频找share--embed，直接copy代码即可。
    
video test 1 beginns： 
   
<iframe width="560" height="315" src="https://www.youtube.com/embed/bty7LHm14CA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
   
   video test ends. 
   
方法二用https://github.com/spaceroam/jekyll-embed-video 这个方法，预先写好框架，用时只要输入视频ID

video test 2 beginns:

{% include youtubePlayer.html id=oQc-2gsjgDg %}

video test 2 ends
