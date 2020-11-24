---
layout: post
title: 리눅스 계정 명령어
date: 2020-02-05 09:28:00
description: 리눅스 계정 명령어
---


#### 계정 확인
{:.no_toc}
~~~
#) chage -l 계정
~~~

#### 계정 만료 변경
{:.no_toc}
~~~
#) chage -M -1 계정
~~~

#### 계정 패스워드 잠김 확인
{:.no_toc}
~~~
#) pam_tally2 --user 아이디
~~~

#### 계정 패스워드 잠김 초기화
{:.no_toc}
~~~
#) pam_tally2 --user 아이디 --reset
~~~

#### 그룹 생성
{:.no_toc}
~~~
#) groupadd -g GID group명
~~~

#### 유저 생성
{:.no_toc}
~~~
#) useradd -d (home directory) -m -g (group name) (user name)
~~~

#### 유저 권한 부여
{:.no_toc}
~~~
#) usermod -g GID (user ID)
~~~
