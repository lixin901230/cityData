cityData
========

最新国家行政区划数据。

结构如下：

	var cityData = [
		{ ------------------------------> 省/特别行政区/直辖市对象
			name: '北京市', -------------> 省/特别行政区/直辖市名称
			sub: [ ---------------------> 省/特别行政区/直辖市下辖的地级市
				{
					name: '东城区', -----> 省/特别行政区/直辖市下辖地级市名称
					sub: [ -------------> 地级市下辖区/县/...
						{name: 'xxx'} --> 区/县/...名称
					]
				}
			]
		}
	];

**数据来源：**

- [国家统计局 - 县及县以上行政区划代码](http://www.stats.gov.cn/tjsj/)
- [百度百科 - 台湾](http://baike.baidu.com/view/2200.htm?fr=wordsearch#5)

> 说明：定期更新[周日]。

暂时不包括比县级以下的划分，也不包括邮政编码等信息。如果有精力，后面考虑整理出来。