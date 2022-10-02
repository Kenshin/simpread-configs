---
title: "我如何使用 Notion 管理简悦的一切"
alias: 
  - "我如何使用 Notion 管理简悦的一切"
created-date: 2022-09-24T16:34:27+0800
type: Simpread
banner: "https://cdn.sspai.com/2021/12/01/316ccb44c2542cfdc492b84faf0e3085.png "
banner_icon: 🔖
tag: 
idx: 2
---

# 我如何使用 Notion 管理简悦的一切

> [!example]- [🧷内部链接](<http://localhost:7026/unread/2>) [🌐外部链接](<https://sspai.com/post/70237>)    
> URI:: [🧷](<http://localhost:7026/unread/2>) [🌐](<https://sspai.com/post/70237>) 
> intURI:: [🧷内部链接](<http://localhost:7026/reading/2>)

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
>  **Description**:: 我每天都要处理两类事务：简悦 & 工作，每个事务都会有不同的角色。通过这篇文章，我就来跟大家分享下使用 Notion 管理简悦的一切工作的经验。
%%

> [!md] Metadata  
> **标题**:: [我如何使用 Notion 管理简悦的一切](https://sspai.com/post/70237)  
> **日期**:: [[2022-09-24]]  

## Annotations


> [!srhl2] [[SR2@我如何使用 Notion 管理简悦的一切|📄]] <mark style="background-color: #ffeb3b">Highlights</mark> [🧷](<http://localhost:7026/unread/2#id=1664008650243>) [🌐](<http://localhost:7026/reading/2#id=1664008650243>)   
> 处理简悦时，除编码以外的大多数事情非常细碎，所以一天下来的日志可能会非常零碎，为了避免这种情况，我「改造」了间歇日记，把它变成了我的工作日志。
> 
> 同时我不会刻意使用番茄工作法来辅助，因为这会让我觉得有些「紧张」。
> 
> 首先我会把任务（ Task ）分得越细越好，这样估算每个工作时间也就越精准。每完成一个 Task 就记录在 Notion 中，当一天下来后，就完成了每天的日志。
> 
> 我会为每个 Small Project 在 Notion 建立一个如下的结构，然后使用 Paste and Sync 的方式嵌入到工作日志（间歇日记）中。
> ^sran-1664008650243

> [!srhl3] [[SR2@我如何使用 Notion 管理简悦的一切|📄]] <mark style="background-color: #a2e9f2">Highlights</mark> [🧷](<http://localhost:7026/unread/2#id=1664008663981>) [🌐](<http://localhost:7026/reading/2#id=1664008663981>)   
> ![](https://cdn.sspai.com/2021/12/01/article/d6027cfdc15580892a6013d9af40ae95)
> ^sran-1664008663981

> [!srhl5] [[SR2@我如何使用 Notion 管理简悦的一切|📄]] <mark style="background-color: #a8ea68">Highlights</mark> [🧷](<http://localhost:7026/unread/2#id=1664008668130>) [🌐](<http://localhost:7026/reading/2#id=1664008668130>)   
> ![](https://cdn.sspai.com/2021/12/01/article/dcf998c9e173632ef816f7fae4165c9b)
> ^sran-1664008668130

