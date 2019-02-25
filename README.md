# 根据K线和量来寻找相似股票
#
# 打开Similar.exe，显示
# ![Image text](https://github.com/l976308589/SimilarKLine/blob/master/Image/1.png)
#1.update:更新历史数据;

#2.get correlation coefficient:寻找相似股票;

#3.setting:设置。
#
#首次使用应该先配置，配置如下图
# ![Image text](https://github.com/l976308589/SimilarKLine/blob/master/Image/2.png)
#其中，有两种选择方式，筛选和特定。筛选功能由1和2组成，为从整个A股市场筛选股票并比对。特定功能为3，以输入的股票为目标，从该目标所在的行业中筛选相似股票。

#1.changeThreshold,%:筛选阈值。当且仅当股票当日的涨幅大于changeThreshold，才会被加入比对。如果想比对所有的股票，changeThreshold填写-100即可。

#2.targetIndustry:目标行业。需要比对的行业，当且仅当股票在设定行业中，才会被匹配。多个行业的话以英文“，”间隔。如果想比对所有行业，填写“All，”即可。

#3.targetStock:目标股票。如果想利用changeThreshold和targetIndustry筛选股票，该字段填写“All，”即可。否则，填写需要比对的股票，此时1和2失效。

#比如筛选“银行”业所有涨幅大于0的股票并比对
# ![Image text](https://github.com/l976308589/SimilarKLine/blob/master/Image/3.png)
#比如仅仅比对“600677”和“600318”
# ![Image text](https://github.com/l976308589/SimilarKLine/blob/master/Image/4.png)

#配置之后点击get correlation coefficient，即可获得结果。
