---
layout: post
title:  regular_expression_example
date:   2020-07-14 13:10:35 +0900
description: regular_expression_example
---
```
평균 계산
data : 64 bytes from 8.8.8.8: icmp_seq=1 ttl=51 time=39.7 ms
command : sed -n 's/^.*time=\(.*\) ms/\1/p' aa | awk '{sum+=$1} END{print sum/NR}'
 - sed : 필터링과 텍스트를 변환하는 스트림 편집기
 - sed -n : 포함한 행만 출력
 - s/^.*time=\(.*\) ms/\1/: "^.*time=\(.*\) ms"을 "\1"로 치환
 - ^.* : 모든 문자열
 - \(.*\) : ( )그룹핑, \(.*\) = (.*) = 모든 문자열
 - \1 : 그룹핑의 매개변수 = \(.*\)
 - p : 출력
 - aa : 파일 명
 - awk : 패턴 탐색과 처리를 위한 명령어
 - {sum+=$1} : 그룹핑의 값들을 더함
 - END{print sum/NR} : 더한 값들의 평균을 계산
```
