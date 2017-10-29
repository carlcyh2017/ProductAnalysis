# ProductAnalysis

项目说明:

    主要是用来练习数据抓取和数据分析,并通过前端页面来显示分析结果,目前只抓取zol中的手机,笔记本,数码相机

    相关知识点放在doc目录,更详细的还是要去官方文档查看

请用IE或Chrome浏览器打开,本人不是做前端的,好像别的浏览器打开有问题

使用步骤:

    1.先mysql数据创建数据库名为:productanalysis,数据库编码一定要设置成utf-8

    2.同步数据库:python manage.py makemigrations 和 python manage.py migrate

    3.进入app/ProductData,执行:run.py

    等待执行结束就可以了

用到技术点:

    1.通过django-haystack来实现全文搜索

    2.直接通过scrapy-redis来实现去重

    3.前端数据分析展示通过bokeh来实现

    4.数据分析用的是pandas
    
    5.通过redis进行缓存处理

##  首页
![](./screen/index.png)
##  分析结果页
![](./screen/search.png)
