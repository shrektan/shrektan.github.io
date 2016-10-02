---
layout: post
title: R Markdown与探索性的研究
---

> But if you never try you'll never know -- Fix you, Coldplay

### 什么是R Markdown

从[R Markdown](http://rmarkdown.rstudio.com)的官网上扒来一段话：

> R Markdown is an authoring format that enables easy creation of dynamic documents, presentations, and reports from R. It combines the core syntax of markdown (an easy to write plain text format) with embedded R code chunks that are run so their output can be included in the final document. R Markdown documents are fully reproducible (they can be automatically regenerated whenever underlying R code or data changes).

总之，它是一个和[IPython](https://ipython.org/notebook.html)比较类似的“环境”，在这个“环境”下，我们能把文本和代码混在一块书写，以一种非常简单的方式形成报告。

### 闲扯

虽然我是[谢大大](http://yihui.name)的粉丝，也一直在使用`knitr`等包生成正规报告，偶尔也会用用`R Markdown`做点Presentation。
但是，却没想过它和“探索型研究”是天然的搭档。

直到前几天，帮阿小福做了个关联分析的[小案例](https://github.com/shrektan/analysis4YZ)时才突然意识到，R Markdown特别适合运用于此类“探索型的研究”：**研究者只需要把精力集中在内容的创造上，其清晰的输出格式又进一步方便了研究者的分析，从而加速了“实验想法 - 分析结果 - 调整设想”的探索型研究回馈路径。**
相较于“改代码 - 看图/数 - 再改代码”的方式，它有两个优点：

1. 分离了“想法实践”和“结果分析”的步骤，使得整个流程更加符合人类思考的天性；
1. 在分析完成后直接保留了所有步骤和结果，有利于后续整理和延展。

我的个神，发现这blog的创作日期是有要求的，即不能大于美帝当前的日期，否则不会显示。好吧，写成3月4日也无妨。
