---
title: "看板、双向链接、知识图谱…… 简悦 2-2 想让你的稍后读不再不读"
alias: 
  - "看板、双向链接、知识图谱…… 简悦 2-2 想让你的稍后读不再不读"
created-date: 2022-09-24T16:38:25+0800
type: Simpread
banner: "https://cdn.sspai.com/article/053250ba-a755-1fb8-25d7-d96ca0aa7b31.png "
banner_icon: 🔖
tag: 
idx: 4
---

# 看板、双向链接、知识图谱…… 简悦 2-2 想让你的稍后读不再不读

> [!example]- [🧷内部链接](<http://localhost:7026/unread/4>) [🌐外部链接](<https://sspai.com/post/67074>)    
> URI:: [🧷](<http://localhost:7026/unread/4>) [🌐](<https://sspai.com/post/67074>) 
> intURI:: [🧷内部链接](<http://localhost:7026/reading/4>)

%%
> [!example]+ **Comments**  
> ```dataview
> TABLE 
>     WITHOUT ID
>     link(Source, dateformat(date(Source), "yyyy-MM-dd")) as Date___, 
>     regexreplace(rows.Comments,"^@@\[\[.+?\]\]\s","") as "Comments"
> FROM "journals"
> WHERE  contains(cmnt, this.file.name)
> FLATTEN cmnt as Comments
> WHERE contains(Comments, this.file.name)
> GROUP BY file.link as Source
> SORT rows.file.day desc
> ```
>  **Description**:: 我希望简悦不仅是一个工具，它更应该是你的信息获取助理，是建立在信息与笔记之间的桥梁，是建立在原始网页与生产力工具之间的桥梁。
%%

> [!md] Metadata  
> **标题**:: [看板、双向链接、知识图谱…… 简悦 2-2 想让你的稍后读不再不读](https://sspai.com/post/67074)  
> **日期**:: [[2022-09-24]]  

## Annotations


> [!srhl2] [[SR4@看板、双向链接、知识图谱…… 简悦 2-2 想让你的稍后读不再不读|📄]] <mark style="background-color: #ffeb3b">Highlights</mark> [🧷](<http://localhost:7026/unread/4#id=1664008720665>) [🌐](<http://localhost:7026/reading/4#id=1664008720665>)   
> 传统的稍后读只是将不同的信息用「文件夹 + 标签」方式来展示，但这样对信息来说，颗粒度还是太大了。简悦对此的解决方案是：**稍后读与标注具有一样的地位，且都可以支持无限层级标签系统**。这样做虽然减小了信息的颗粒度问题，但并未真正解决信息的关联性问题。
> 
> 随着 Zettelkasten 笔记法的流行，越来越多的使用者开始注意笔记（信息）之间的内化与相互之间的关联性，其实在 Wiki 页面就存在着这样的信息关联性，而作为信息完整度最好的稍后读工具，却天然地缺失这类方式。
> 
> 因此 2.2.0 版简悦的稍后读借鉴了 ZK 笔记法的一些特点，专门针对信息的整合增加了如下一些新功能，对于一个稍后读产品来说这些功能都是简悦独有的功能。
> 
> *   [双向链接](http://ksria.com/simpread/docs/#/%E5%8F%8C%E5%90%91%E9%93%BE%E6%8E%A5)
> *   [知识图谱](http://ksria.com/simpread/docs/#/%E5%8F%8C%E5%90%91%E9%93%BE%E6%8E%A5?id=%E5%9B%BE%E8%B0%B1)
> *   [Mindmap](http://ksria.com/simpread/docs/#/%E7%A8%8D%E5%90%8E%E8%AF%BB?id=Mindmap)
> *   多种信息展示方式（布局）：[Evergreen](http://ksria.com/simpread/docs/#/%E7%A8%8D%E5%90%8E%E8%AF%BB-%E5%A4%9A%E7%A7%8D%E5%B8%83%E5%B1%80?id=Evergreen)、[Workflowy](http://ksria.com/simpread/docs/#/%E7%A8%8D%E5%90%8E%E8%AF%BB-%E5%A4%9A%E7%A7%8D%E5%B8%83%E5%B1%80?id=Workflowy)、[k](http://ksria.com/simpread/docs/#/%E7%A8%8D%E5%90%8E%E8%AF%BB-%E5%A4%9A%E7%A7%8D%E5%B8%83%E5%B1%80?id=Kanban)
> ^sran-1664008720665

> [!srhl6] [[SR4@看板、双向链接、知识图谱…… 简悦 2-2 想让你的稍后读不再不读|📄]] <mark style="background-color: #ffb7da">Highlights</mark> [🧷](<http://localhost:7026/unread/4#id=1664008727659>) [🌐](<http://localhost:7026/reading/4#id=1664008727659>)   
> ![](https://cdn.sspai.com/2021/05/27/3df7b554b18a30e156673c3511a897e2.png)
> ^sran-1664008727659

> [!srhl4] [[SR4@看板、双向链接、知识图谱…… 简悦 2-2 想让你的稍后读不再不读|📄]] <mark style="background-color: #a1e0ff">Highlights</mark> [🧷](<http://localhost:7026/unread/4#id=1664008742365>) [🌐](<http://localhost:7026/reading/4#id=1664008742365>)   
> ### 新的布局
> 
> 布局是信息的展示方式，加入了双向链接等功能后，2.2 版本之前的布局已经无法承载这些内容。所以 2.2 版本增加了三类布局：
> 
> *   [Evergreen](http://ksria.com/simpread/docs/#/%E7%A8%8D%E5%90%8E%E8%AF%BB-%E5%A4%9A%E7%A7%8D%E5%B8%83%E5%B1%80?id=Evergreen)：信息的之间的关联性联系
> *   [Workflowy](http://ksria.com/simpread/docs/#/%E7%A8%8D%E5%90%8E%E8%AF%BB-%E5%A4%9A%E7%A7%8D%E5%B8%83%E5%B1%80?id=Workflowy)：将多种信息汇总为一个页面
> *   [Kanban](http://ksria.com/simpread/docs/#/%E7%A8%8D%E5%90%8E%E8%AF%BB-%E5%A4%9A%E7%A7%8D%E5%B8%83%E5%B1%80?id=Kanban)：用 GTD 的方式管理你的稍后读
> ^sran-1664008742365

