# 冲顶大会/百万赢家/头脑王者/UC疯狂夺金答题辅助：抓包获取题目并搜索答案
冲顶大会/百万赢家/头脑王者/UC疯狂夺金：抓包获取题目，不用图像识别:)

测试环境：Kali Linux,Python3，Android

需要的抓包工具：[mitmdump](https://github.com/mitmproxy/mitmproxy)

[mitmdump官方文档](http://docs.mitmproxy.org/en/stable/index.html)

## 使用方法
[mitmproxy安装方法](http://docs.mitmproxy.org/en/stable/install.html)

首次运行`mitmdump`或`mitmproxy`，在`.mitmproxy/`中获取证书`mitmproxy-ca-cert.cer`

在Android手机中安装证书，与电脑处于同一wifi下，手动设置代理为电脑ip地址：192.168.1.100，端口（默认）：8080

	git clone https://github.com/vanpersiexp/chongding.git
    cd chongding/
	pip3 install -r related.txt
	mitmdump -s get_question.py
	python3 search_question.py -h
	
	usage: search_question.py [-h] [-b {1,2,3,4}]

	冲顶大会/百万赢家/头脑王者/UC疯狂夺金:抓包获取题目并搜索答案。

	optional arguments:
  	-h, --help            		show this help message and exit
  	-b {1,2,3,4}, --brand {1,2,3,4}		
					选择APP，1：冲顶大会；2：百万赢家；3：头脑王者；4：UC疯狂夺金
	

## 抓包结果
冲顶大会抓包结果：
![冲顶大会](https://raw.githubusercontent.com/vanpersiexp/chongding/master/img/20180126_17.jpg)

头脑王者抓包结果：
![头脑王者](https://raw.githubusercontent.com/vanpersiexp/chongding/master/img/tounaowangzhe.jpg)

UC疯狂夺金抓包结果：
![疯狂夺金](https://raw.githubusercontent.com/vanpersiexp/chongding/master/img/fkdj_2.jpg)

## 运行效果
可以使用`example/`中的抓取的数据包测试程序。
实时运行效果如图：

冲顶大会：

![冲顶大会](https://raw.githubusercontent.com/vanpersiexp/chongding/master/img/chongdingdahui.jpg)

百万赢家：

![百万赢家](https://raw.githubusercontent.com/vanpersiexp/chongding/master/img/baiwanyingjia.jpg)

头脑王者：
![头脑王者](https://raw.githubusercontent.com/vanpersiexp/chongding/master/img/tounao.jpg)

UC疯狂夺金：
![疯狂夺金](https://raw.githubusercontent.com/vanpersiexp/chongding/master/img/fkdj_1.jpg)

## 联系方式
pu.xiaorvp@gmail.com
