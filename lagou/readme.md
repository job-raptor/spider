# 抓取拉勾的职位信息

#### 页面分析

页面分成index和详情两类

详情页比较简单,形如 `https://www.lagou.com/jobs/3750177.html` 需要解决的问题是:

- 反爬问题,主要通过UA变化,cookie写入,换IP等方式解决
- https问题,用requests或scrapy都好解决

index页即,形如`https://www.lagou.com/zhaopin/PHP/` 需要解决的问题是:

- index页面的数据接口目前还没找到,他人代码中的内容目前看来都已被拉勾干掉
- 抓取哪些分栏目（本质上是搜索页）
