---
layout: post
title:  _posts 경로 markdown 생성 스크립트
date:   2020-11-24 20:01:52 +0900
description: _posts 경로 markdown 생성 스크립트
---


#### Code
{:.no_toc}
~~~
#!/bin/bash

#date=`date +%Y-%m-%d`
date=$(date '+%Y-%m-%d')
datet=$(date '+%Y-%m-%d %H:%M:%S')

gitpath= _posts 파일 경로

if [ $# -ne 1 ]; then
            echo "Usage: $(basename $0) <title>"
                exit 99
        fi

        title=$1

        path=$gitpath/$date-$title.md

touch $path

cat <<__EOF__>> $path
---
layout: post
title:  $title
date:   $datet +0900
description: $title
---
__EOF__
~~~
