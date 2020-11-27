# statistic_analysis_for_price_data

这是一个对价格时间序列进行统计分析的工具。

this is a tool used to do statistic analysis for time series with price

对于一个时间超过三年的价格时间序列，短时间里人脑是很难处理完成的，把图放大了看不到局部、不知道具体价格，把图缩小了又容易一叶障目，还有如何用肉眼去区别不同年份的价格情况等等，都是常人难以做到的。

于是为了快速了解一个时间序列的基本情况，写了下相关的代码，可以快速统计一个表格里的时间序列信息，详细的结果与应用可以看[这篇文章](https://mp.weixin.qq.com/s/pBtztysOJsogvmog6wbxJA).

For a price time series of more than three years, it is difficult for the human brain to process it in a short time, and it is hard for ordinary people to zoom in the graph to see the local and specific prices, and zoom out the graph to see the price in a blurred view, and how to distinguish the price situation of different years with the naked eye.

So in order to quickly understand the basic situation of a time series, I wrote the following related code, which can quickly count the time series information in a table, and detailed results and applications can see [this article](https://mp.weixin.qq.com/s/pBtztysOJsogvmog6wbxJA).

### 如何使用

1. **环境**：有一个基于python的编程环境(可以使用anaconda)，使用jupyter打开ipynb文件。
2. **数据文件**：将数据文件放在.ipynb文件同目录下，里面请不要有冗余行列，请按照`Date, Open, High, Low, Close, Volume, Market Cap`排列(尽管只用到了Date和Close)，区分大小写，有自己需求的请自行改写。
3. **修改symbol**：将symbol后面赋值为数据文件名称，按相应按键运行即可。

### How to use

1. **Environment**: You have a python based programming environment (you can use anaconda), use jupyter to open the ipynb file. 
2. **Datafiles**: Put the datafiles in the same directory as the .ipynb file, no redundant rows and columns, please arrange them according to `Date, Open, High, Low, Close, Volume, Market Cap` (although only Date and Close are used), case sensitive. You can rewrite it yourself. 
3. **Modify symbol**: Assign the symbol followed by the data file name, press the corresponding key to run.

### 可以做什么

1. 基础统计分析(日收益率最大值、日收益率最小值、日单向波动大于10%的时间与幅度、阳线数量、阴线数量、最大连续上涨笔数、最大连续下跌笔数)
2. 连续盈亏天数柱状图
3. 日收益率波动图、月收益率波动图
4. 收益率分布图
5. 大收益率时间分布图
6. 年周期图
7. 月均收益率与胜算图
8. 月累计收益率图
9. 循环分析诸多品种的数据

### What can be done

1. basic statistical analysis (maximum daily yield, minimum daily yield, duration and magnitude of daily one-way fluctuations greater than 10%, number of positive lines, number of negative lines, maximum number of consecutive up trades, maximum number of consecutive down trades)
2. a histogram of the number of consecutive days of profit and loss.
3. daily and monthly yield volatility charts
4. yield distribution chart
5. time distribution of large yields
6. annual cycle chart
7. average monthly returns and odds charts
8. monthly cumulative yield chart
9. cyclic analysis of data from many species

### 接下来可能更新什么

- 其中计算连续盈亏天数的代码运行速度较慢，以期优化
- 由于最初是写来统计比特币数据的，对于有涨跌停板制度的商品期货而言，部分地方考虑欠缺，以期优化
- 生成更多的数据(**有其他感兴趣的数据可以留言**)
- 制作成html，方便没有编程基础与环境的人使用


### What might be updated next?

- The code that calculates the number of consecutive days of profit and loss is slow, in order to optimize it.
- As it was originally written to compile bitcoin statistics, some aspects of commodity futures, which have a halt-and-stop system, are not being considered for optimization.
- Generate more data (**Please leave a comment if you have other data of interest**).
- Create html for people with no programming background or environment.
