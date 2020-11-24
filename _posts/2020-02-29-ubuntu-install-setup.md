---
layout: post
title: 우분투 다운로드 서버 확인
date: 2020-02-09 10:25:00
description: 우분투 다운로드 서버 확인
---

#### 우분투 다운로드 서버 확인
{:.no_toc}

~~~
#) cat /etc/apt/sources.list
~~~

#### 우분투 다운로드 서버 변경
{:.no_toc}

~~~
#) sudo sed -i 's/archive.ubuntu.com/ftp.daum.net/g' /etc/apt/sources.list
~~~
