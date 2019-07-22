---
title: Conan（五）：Uploading Packages
date: 2019-07-21 23:27:39
description: Conan
tags:
- C/C++
- 包管理
categories:
- Conan
image: post/201907/Conan_Uploading_Packages/conan_upload_package.png
---

## 0x0 Remotes

**可供选择的server**
For private develepment
- Artifactory Community Edition for C/C++ （详见[Conan（二）：使用Artifactory搭建私仓](http://hanxiatu.com/post/201907/Conan_localrepo.html)）
- Artifactory Pro
- Conan server

For distribution
- [Bintray](https://docs.conan.io/en/latest/uploading_packages/using_bintray.html#using-bintray)

## 0x1 上传包到 Remotes
```
conan remote list

conan remote add my_local_server http://localhost:9300

conan search [xxx] -r=my_local_server

conan upload xxx --all -r=my_local_server
```

## 0x2 参考链接
1. [Conan：Uploading Packages](https://docs.conan.io/en/latest/uploading_packages.html)