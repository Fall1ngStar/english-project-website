---
layout: post
title:  "Import planning"
date:   2019-03-06 14:00:00 +0100
categories: golang discovery
---

## Work environment :

I don't have a personal laptop and we are not allowed to intall programme on the computers of the university. So the problem is that i can't install softwares we needs (**Golang**) to programme our project. To slove this problem i have to do my changes of codes with an **integrated online development environment**. So i will use **AWS Cloud9** which can do that.

**Golang** is a new programming language for me, I never used it before. So I learned the basics of this language, with the website **A Tour of Go**, in order to be able to programming with this technology.

## Import planning :

I have to do functions that will allow to **import the weekly and daily planning**, which are on the site of the university, according to the dates enter in parameters.
Then i have to parse the import to **String**. The method must **returns a String** to extract datas we need later.

#### To realize this, i did 2 functions :

```go
func GetWeeklyPlanning(yearMonthDayStart string, yearMonthDayEnd string) string {}
```
**and**
```go
func GetDailyPlanning(yearMonthDay string) string {}
```
These functions generate a **url** and call another function with this url in parameter to **download and parse in string** the planning.

*Made by elliot*
