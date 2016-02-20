---
layout: post
title: Want to be a contributor to the R Community
---

从2013年正式学习R到现在，正好三年时间。虽然说R的诞生早在20多年前，但这三年里，却算得上是R Community 发展最为迅猛的时期，基本上，每周都会见证让人激动新功能的产生。在工作中，每次做出各种满意的功能，我都会对贡献相关代码的神人们心生感激，也会希望自己能对他人有所帮助，权当作自己对于R Community的回馈吧。

从去年开始，工作中的代码都尽量以package的形式去封装。经过近一年的锻炼，觉得自己还算熟练掌握了R pacakge的开发。加上各种编程基础知识的恶补，隐约感到可能也许不久的将来，自己也会慢慢地写大块的pull request，也会写出一两个精于某项小功能的包，为整个社区贡献出自己的力量。

Let's see.

目前觉得自己可能会做的两个事情是：

- __关于商业表格（business reporting table）的生成：__{: style="color: red"} 对于商业表格的生成，目前还没有什么特别好的解决方式。`DT`对于通用型的html表格显示非常棒，但实现起商业报告类的表格（row based formating），仍然比较繁琐。`formattable`也是一个不错的包，但感觉还没有`DT`好用。`xtable`只在pdf生成时还比较顺手。另外还有一个问题是，`DT`和`formattable`都不能提供对应pdf表格的生成，而商业表格往往需要生成pdf的报告。我暂时的做法是在网页中用`DT`，在pdf中就`xtable`。但仍存在两个问题：一是重复、二是对于某些复杂的格式，设置极为繁琐。__希望今年能有余力做一个包出来，彻底解决此问题。__
- __The R interface of Echarts：__{: style="color: red"} [Echarts](http://echarts.baidu.com)是一个纯 Javascript 的图表库和[highcharts](http://www.highcharts.com)类似。前年刚看到这个项目时，心中确实是激动了一番（之前没有见过交互方式如此灵活的图表），当时很想做个R的interface，但限于当时的功底和时间便放弃了。现在觉得技术方面可能足够了（主要由于[htmlwidgets](http://htmlwidgets.org/)的发展），而且yihui开了个[好头](https://github.com/yihui/recharts)。不过，除我个人时间可能不够外，[highcharter](https://github.com/jbkunst/highcharter)和其他d3图表库的出现（如dygraphs, streamgraphs等）让我觉得这个想法似乎没有那么必要了…… 所以再看吧……

该去跑步了~ :D

