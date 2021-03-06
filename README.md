# CryptoLib
![MIT License](https://img.shields.io/badge/License-MIT-red.svg)
![C++](https://img.shields.io/badge/Language-C%2B%2B-brightgreen.svg)
![Version](https://img.shields.io/badge/Version-1.0-blue.svg)
[![Build status](https://ci.appveyor.com/api/projects/status/pgqrs47g0cec0k2g?svg=true)](https://ci.appveyor.com/project/MXWXZ/cryptolib)

CryptoLib是一个轻量级C++密码类库，完全编译只需要几十KB！包括常用哈希、加解密、硬件信息获取、拓展类等模块，基于MIT协议，可以用于商业软件。

帮助文档：<https://mxwxz.github.io/CryptoLib/>

# 支持的模块
常用哈希：
MD5 SHA1 SHA256 SHA512 CRC32(Poly：0xEDB88320L)

常用加解密：
Base64 UrlEncode(RFC3986)

硬件信息：
硬盘序列号 MAC地址 CPU序列号 主板序列号 BIOS序列号

拓展类：
字符串类 大数类

# 简单地使用

``` 
HashClass::Generate(str)                        //计算str哈希值，默认返回小写
HashClass::GenerateFile(_T("File Name")));      //计算文件哈希，默认返回小写
EncodeClass::Encode(str);                       //加密
EncodeClass::Decode(str);                       //解密
InfoClass::GetSN();                             //取得序列号
```


# 鸣谢
在开发过程中，少不了下面的开源代码的支持：

ulwanski：https://github.com/ulwanski/md5

ulwanski：https://github.com/ulwanski/sha512

vog：https://github.com/vog/sha1

黑猫崽儿：http://blog.csdn.net/c_duoduo/article/details/43889759

陈秋树：http://blog.sina.com.cn/s/blog_57dff12f0100d5sn.html

liruda：http://blog.csdn.net/liruda/article/details/2254378
