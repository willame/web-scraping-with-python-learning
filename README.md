# web-scraping-with-python-learning
web-scraping-with-python-learning book source


## Python 网络爬虫 011 (高级功能) 支持代理proxy — 让爬虫可以翻墙爬取网站

### 支持代理

- 使用的系统：Windows 10 64位 (在ubuntu14.04上面运行报错)
- Python 语言版本：Python 2.7.10 V
- 使用的编程 Python 的集成开发环境：PyCharm 2016 04
- 我使用的 urllib 的版本：urllib2
- 注意： 我没这里使用的是 Python2 ，而不是Python3

我们可以使用 urllib2 支持代理

'''
proxy = ...
opener = urllib2.build_opener()
proxy_params = {urlparse.urlparse(url).scheme: proxy}
opener.add_handler(urllib2.ProxyHandler(proxy_params))
response = opener.open(request)
'''


[原文传送门](http://www.aobosir.com/blog/2016/12/25/python-Web-crawler-proxy-support/)
