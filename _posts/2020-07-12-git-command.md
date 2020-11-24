---
layout: post
title:  git 명령어
date:   2020-07-12 21:41:30 +0900
description: git 명령어
---
```
git add *
git commit -m "first blog update"
git push -u origin master

git config --list
git config --global user.name "userid"
git config --global user.email "user@email.com"

warning: LF will be replaced by CRLF in _posts/2020-07-14-Regular_expression.markdown.
The file will have its original line endings in your working directory
 → Whitespace 에러, 유닉스 시스템에서는 한 줄의 끝이 LF(Line Feed)로 이루지기 때문에
   git에게 혼란을 줌
   해결 : git config --global core.autocrlf true

```
