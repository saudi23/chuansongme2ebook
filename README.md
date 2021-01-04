# chuansongme to ebook
A python script to convert chuansongme.com (wechat official accounts mirror) to ebook.

Use kindlegen or calibre to pack package.opf to ebook.
我花了点时间写了这样一个脚本，可以把微信公众号在传送门上的镜像抓取下来生成电子书。

之所以选择爬传送门，是因为听说腾讯反爬虫很严厉。

源代码在此： [url]https://github.com/fqx/chuansongme2ebook[/url]

这个脚本重用了很多我之前另一个项目的代码，因此明显可以看得出来变量命名规则的改变。

我也尝试着用面向对象的方式来写这个脚本，虽然不是很成功。

比较值得高兴的是，这次完成了对图片的处理，方法比之前预期的要简单一些。

对微信公众号这种图片比较多的平台特别有意义。

解析部分（simplify_html 函数）针对我要抓的那个公众号做了优化，各位可根据自己的实际需求修改。

爬完后用kindlegen可以生成mobi格式的电子书。

会python的自己爬，本人忙不接受代爬的请求。


2019-04-26更新：支持仅抓取指定时期的文章
