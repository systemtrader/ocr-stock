# ocrstock
ocrstock是使用python模拟鼠标操作实现股票自动化交易的程序。

# ocr
也就是使用ocr技术识别图像，屏幕截图内容，实现图像数据提取，定位等内容。

数据提取使用的不是ocr技术，而是深度学习和数据挖掘技术，其中在ml下面已经完成数字串的识别，可以直接调用该训练好的模型即可。

而图像定位，目前使用的模板匹配方式，虽然粗暴，但是有效，简单，缺点是，对于全屏幕范围的匹配时间显得过长。因此在config中时限限定了搜索的范围。

# stock
与股票交易相关。

需要说明的是，这个项目只是自娱自乐，并不能使用在实盘交易中，为什么，因为不稳定啊，速度不够快，虽然比手工快很多，但是真的没有人智能。我测试过了，时间主要耗费在图像信息定位上，而且是全屏幕搜索耗费了大部分时间。

当然，如果你只是小散户，持股不过三五只，或者最多不过七八只，还是可以用的。

# server
server中定义了简单的web服务器，用于接受量化研究平台回传的交易信号，很简单，但是作为只用来接受数据回传，还是很不错的。

待信号回传后，就可以根据这些信号进行买卖操作了。

# note
每个代码文件后面都有test，具体使用请参考test。


苏振裕

20170916
