---
title: git10054
date: 2022-12-05 22:32:28
tags: git
categories: git
---

### git 443 10054报错
``` bash
fatal: unable to access 'https://github.com/whywherewhatwhen/myblog.git/': Failed to connect to github.com port 443 after 21067 ms: Timed out 
```
github连不上 超时

``` bash
fatal: unable to access 'https://github.com/whywherewhatwhen/myblog.git/': OpenSSL SSL_read: Connection was reset, errno 10054
```

``` bash
git config --global http.sslVerify "false"
```
把http.sslVerify 设置为false