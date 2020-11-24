---
layout: post
title: OS 스펙 확인
date: 2020-02-09 10:09:00
description: OS 스펙 확인
---

REDHAT LINUX 기준

#### OS 정보
{:.no_toc}
~~~
#) cat /etc/redhat-release
~~~

#### OS BIT 정보
{:.no_toc}
~~~
#) getconf LONG_BIT
~~~

#### memory 정보
{:.no_toc}
~~~
#) cat /proc/meminfo
~~~

#### cpu 정보
{:.no_toc}
~~~
#) cat /proc/cpuinfo
~~~

<hr>
<br/>

AIX 기준

#### OS 정보
{:.no_toc}
~~~
#) uname -r
~~~

#### OS BIT 정보
{:.no_toc}
~~~
#) /bin/isainfo -kv
~~~

#### memory 정보
{:.no_toc}
~~~
#) prtconf | grep memory
~~~

#### cpu 정보
{:.no_toc}
~~~
#) psrinfo -p
~~~
