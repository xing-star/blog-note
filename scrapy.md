#### 安装Scrapy错误：Microsoft Visual C++ 14.0 is required...

##### 问题描述

- 环境：win10，python3.4.4，64位

- 在windows下，在dos运行pip install Scrapy报错。
`
 error: Microsoft Visual C++ 10.0 is required (Unable to find vcvarsall.bat).
`

##### 解决方案

- http://www.lfd.uci.edu/~gohlke/pythonlibs/#twisted 下载twisted对应版本的whl文件（如我的Twisted‑17.5.0‑cp36‑cp36m‑win_amd64.whl），cp后面是python版本，amd64代表64位，运行命令：

`
pip install whl文件的完整路径名
`

- 安装完成后再次运行：
`
pip install Scrapy
`
- 即可成功


#### 执行爬虫的时候`scrapy crawl 爬虫名`提示`ImportError: No module named 'win32api'`

##### 解决方案

`
解决办法：安装pywin32
地址：https://sourceforge.net/projects/pywin32/files/pywin32/Build%20220/
`

- 安装成功之后重试scrapy crawl 爬虫名即可成功
