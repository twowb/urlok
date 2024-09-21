欢迎关注【蓝记战队】WX公众号，这里有最新最前沿的干活技术，不搬运不玩低端LOW炮的东西是我们的宗旨！！！

针对空间引擎出来的大量结果进行存活探测

```
▗▖ ▗▖▗▄▄▖ ▗▖    ▗▄▖ ▗▖ ▗▖
▐▌ ▐▌▐▌ ▐▌▐▌   ▐▌ ▐▌▐▌▗▞▘
▐▌ ▐▌▐▛▀▚▖▐▌   ▐▌ ▐▌▐▛▚▖ 
▝▚▄▞▘▐▌ ▐▌▐▙▄▄▖▝▚▄▞▘▐▌ ▐▌
                         - 一个简单的URL可用性测试工具
作者：zngeek
版本：1.0.0

Usage of ./urlok:
  -c string
    	期望的HTTP状态码，多个状态码用逗号分隔，默认为200和301 (default "200,301")
  -f string
    	URL文件路径，每行一个URL
  -o string
    	输出结果文件，每行一个可以访问的URL (default "output.txt")
  -p string
    	代理服务器地址，支持socks5和http代理，如：socks5://127.0.0.1:1080 或 http://127.0.0.1:8080
  -q	如果设置为true，则移除重复的URL，默认false
  -t int
    	并发线程数，默认为10 (default 10)
```

目前编译了如下架构

```
-rwxrwxr-x 1 zngeek zngeek 4.8M  9月 21 22:40 urlok_darwin_amd64
-rwxrwxr-x 1 zngeek zngeek 4.7M  9月 21 22:40 urlok_darwin_arm64
-rwxrwxr-x 1 zngeek zngeek 4.6M  9月 21 22:39 urlok_linux_386
-rwxrwxr-x 1 zngeek zngeek 4.7M  9月 21 22:39 urlok_linux_amd64
-rwxrwxr-x 1 zngeek zngeek 4.6M  9月 21 22:39 urlok_linux_arm64
-rwxrwxr-x 1 zngeek zngeek 4.8M  9月 21 22:40 urlok_windows_386.exe
-rwxrwxr-x 1 zngeek zngeek 5.0M  9月 21 22:40 urlok_windows_amd64.exe
-rwxrwxr-x 1 zngeek zngeek 4.7M  9月 21 22:40 urlok_windows_arm64.exe
```

```
55bb786532e125e984279c541afb6b92  urlok_darwin_amd64
3546819dd873c2c990d0286a8860af08  urlok_darwin_arm64
f359a85773794df3506db69d610312f0  urlok_linux_386
c08735001e052ebcb83278237b1bb35b  urlok_linux_amd64
b2d90deddea25ee8c5ac2dd78b69f18e  urlok_linux_arm64
bfe1f882c55c73c09238b708bf20a6f1  urlok_windows_386.exe
cc113b37a9dd6f472b1985db0a1d1d9a  urlok_windows_amd64.exe
c54e3b9fc59dd2545b9ac654cda6d3a2  urlok_windows_arm64.exe
```

