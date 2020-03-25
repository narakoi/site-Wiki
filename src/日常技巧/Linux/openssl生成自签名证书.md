---
layout: post
title: 使用 openssl 生成自签名证书
slug: generate-self-signed-cert-with-openssl
date: 2020-03-01 13:15
status: publish
author: 熊猫小A
categories: 
  - 
tags:
  - 技巧
  - Linux
  - SSL 
excerpt: 生成自签名证书用于调试
---

通过 openssl 生成私钥 server.key：

```bash
openssl genrsa -out server.key 1024
```

根据私钥生成证书申请文件 csr：

```bash
openssl req -new -key server.key -out server.csr
```

根据提示输入各项参数。Common Name 这一项可以填通配符域名。

使用私钥签名生成证书 server.crt：

```bash
openssl x509 -req -in server.csr -out server.crt -signkey server.key -days 3650
```

有效期 3650 天。自己调试开发足够了。