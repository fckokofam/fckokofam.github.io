---
layout: post
title: apache-tomcat connector
date: 2020-07-03 10:25:00
description: apache-tomcat connector
---

LoadModule 주석 해제

{% highlight c++ %}

LoadModule proxy_module modules/mod_proxy.so
LoadModule proxy_http_module modules/mod_proxy_http.so

{% endhighlight %}

VirtualHost 생성

{% highlight c++ %}

<VirtualHost *:8000>
    ServerName admin@wisoft.com
    ErrorLog "logs/admin@wisoft.com-error_log"
    CustomLog "logs/admin@wisoft.com-access_log" common

    ProxyRequests Off
    ProxyPreserveHost On

    <Proxy *>
	   Order deny,allow
	    Allow from all
    </Proxy>

    ProxyPass / http://192.168.0.32:8080/
    ProxyPassReverse / http://192.168.0.32:8080/
</VirtualHost>

{% endhighlight %}
