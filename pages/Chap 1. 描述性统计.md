- # 1.1 描述统计量
	- ## 1.1.1 位置与分散程度的度量
	  id:: 642b09a4-2bad-4f9e-acef-0920ca956840
		- ### 各种中间值
			- [均值]([[mean]])
			  id:: 642b09d4-6b52-4500-9ed0-f46fec38efec
			  collapsed:: true
				- 数列的算术平均值，反应了数列的集中趋势,等于有效数值的合除以有效数值的个数
			- [中位数]([[median]])
			  id:: 643580a6-150a-44a1-8580-72d5db1e0945
			  collapsed:: true
				- 等于排序后中间位置的值，当数列长度为偶数时，取中间两个值的均值
			- [众数]([[mode]])
			  collapsed:: true
				- 等于数列出现次数最多的数字，当多个数字都出现最高次数时，多个数字都是众数
		- ### 各种平均数
			- [算数平均数]([[arithmetic mean]])
			- [总体均值]([[population mean]])
			  collapsed:: true
				- 简称**期望**，是描述随机变量取值平均状况的数字特征。包括 [离散型随机变量](https://baike.baidu.com/item/%E7%A6%BB%E6%95%A3%E5%9E%8B%E9%9A%8F%E6%9C%BA%E5%8F%98%E9%87%8F/9980865?fromModule=lemma_inlink) 的总体均值和连续型随机变量的总体均值。
			- [几何平均数]([[geometric mean]])
			  collapsed:: true
				- 用于计算增长率或平均利率。
			- [调和平均数]([[harmonic mean]])
			  collapsed:: true
				- 用于计算平均速度或电阻的平均数。
			- #+BEGIN_TIP
			  算数平均数 ≥ 几何平均数 ≥ 调和平均数
			  #+END_TIP
		- ### 数据的离散程度
			- 分位数
			  collapsed:: true
				- [四分位数]([[quartile]])
				  collapsed:: true
					- 将数据按从小到大的顺序排列并分成四等份时，位于各个分割点的数值。
				- ((643580a6-150a-44a1-8580-72d5db1e0945))
				  collapsed:: true
					- 按顺序排列的一组数据中位于正中间的数。不易受离群值的影响。
				- [[四分位距]]
				  collapsed:: true
					- 第三四分位数与第一四分位数的差。数据越向中位数集中，四分位距就越小。
				- [百分位数]([[percentile]])
				  collapsed:: true
					- 如果将一组数据从小到大排序，并计算相应的累计百分位，则某一百分位所对应数据的值就称为这一组数的百分位数
			- **偏差**  Deviation  ？ Bias？ #why
			  collapsed:: true
				- 表示的是每个数据与平均数的差
			- [方差]([[variance]])
			  collapsed:: true
				- 衡量离散程度的指标。用来衡量样本偏离均值的程度，或者描述数据取值分散性程度一个度量。
			- [标准差]([[standard deviation]])
			  collapsed:: true
				- 方差的算术平方根，用衣示。标准差也被称为标准偏差，或者实验标准差，在概率统计中最常使用作为统计分散分布䅣度 上的测量依据。在概率统计中最常使用作为测量一组数值的离散程度之用。
			- [标准误差]([[standard error]])
			  collapsed:: true
				- 描述平均数抽样分布的离散程度及衡量平均数抽样误差大小的尺度，反映样本平均数之间的变异。
			- **离群值**
			- [变异系数]([[coefficient of variation]])
			  collapsed:: true
				- 标准差与平均数的比。用于比较单位不同的样本之间的离散程度。
## 1.4 变量的相关性
	- **等级相关系数**（coefficient of rank correlation）：测量两个定序变量之间相关程度的指标。等级相关系数中有斯皮尔曼等级相关系数和肯德尔等级相关系数。具体使用哪一个，没有明确的基准。
	- **皮尔逊积矩相关系数**（Correlation - Pearson）
		- 相关系数（coefficient of correlation）…表示两个变量之间的关联（相关）程度的指标。相关系数越接近 1，正相关就越强；越接近 -1，负相关就越强；0 表示不相关。
	- $$r = \frac{{}\sum_{i=1}^{n} (x_i - \overline{x})(y_i - \overline{y})}
	  {\sqrt{\sum_{i=1}^{n} (x_i - \overline{x})^2(y_i - \overline{y})^2}}$$
	- **斯皮尔曼等级相关系数**（Correlation - Spearman）
		- 被观测的两个变量的等级的差值 $d_i = x_i - y_i$
		- $$\rho = 1- {\frac {6 \sum d_i^2}{n(n^2 - 1)}}$$
	- **肯德尔等级相关系数**
## 1.4 变量的相关性
collapsed:: true
	- **等级相关系数**（coefficient of rank correlation）：测量两个定序变量之间相关程度的指标。等级相关系数中有斯皮尔曼等级相关系数和肯德尔等级相关系数。具体使用哪一个，没有明确的基准。
	- **皮尔逊积矩相关系数**（Correlation - Pearson）
		- 相关系数（coefficient of correlation）…表示两个变量之间的关联（相关）程度的指标。相关系数越接近 1，正相关就越强；越接近 -1，负相关就越强；0 表示不相关。
	- $$r = \frac{{}\sum_{i=1}^{n} (x_i - \overline{x})(y_i - \overline{y})}
	  {\sqrt{\sum_{i=1}^{n} (x_i - \overline{x})^2(y_i - \overline{y})^2}}$$
	- **斯皮尔曼等级相关系数**（Correlation - Spearman）
		- 被观测的两个变量的等级的差值 $d_i = x_i - y_i$
		- $$\rho = 1- {\frac {6 \sum d_i^2}{n(n^2 - 1)}}$$
	- **肯德尔等级相关系数**
- # 2.概率分布
  collapsed:: true
	- ## 2.1 概率
		- **随机变量**（random variable）：用概率定义要取的值有多容易出现的变量。
	- ## 2.2 概率分布（probability distribution）
		- 连续型分布
			- 均匀分布
			- 离散均匀分布
				- 当值为 [插图] 时，平均数为 [插图]，方差为
				- #+BEGIN_EXPORT latex
				  \rho = 1- {\frac {6 \sum d_i^2}{n(n^2 - 1)}}
				  #+END_EXPORT
-