---
layout: post
title: 视频测试
date: 2020-11-02
Author: 七弦
tags: Test Youtube
youtubeId: bty7LHm14CA
---

测试插入youtube视频。

方法一在Youtube视频找share--embed，直接copy代码即可。
    
video test 1 beginns： 
   
<iframe width="560" height="315" src="https://www.youtube.com/embed/bty7LHm14CA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
   
   video test ends. 
   
方法二用https://github.com/spaceroam/jekyll-embed-video 这个方法，预先写好框架，用时只要输入视频ID

video test 2 beginns:

{% include youtubePlayer.html id=page.youtubeId %}

video test 2 ends

第一次测试方法二失败，成功显示视频框架但无法播放。再试一次。
第一次是直接输入id，第二次改用原文中输入变量的方法。理论上应该一样，再碰碰运气吧。

哈，用了变量竟然成功了。所以之前是输入ID的方法不对？我再来试一遍：

方法三，ID加引号

video test 3 beginns:

{% include youtubePlayer.html id="bty7LHm14CA" %}

video test 3 ends.

这次成功了！果然是这个错误。而昨天之所以不成功就还是那个隔离行的问题。

最后再来试一下responsive框架，也成功了！要把这段代码放到stylesheet也就是style.css里，我昨天直接放在根目录当然没用。不过只针对方法二三，方法一直接嵌入对此无反应。所以本来觉得直接嵌入更方便，以后还是要使用这个方法更好。
