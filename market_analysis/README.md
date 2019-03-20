会员活动数据营销预测
=======================
#项目描述
---
通过现有会员营销活动数据预测在下一次营销活动的会员响应名单和响应概率，以此来制定针对性的营销策略。

#项目数据
---
数据记录数:48000<br>
特征数:13<br>
是否有NA值:有<br>
是否有异常值:无<br>
以下是数据集的13个特征变量:<br>
  1.age:年龄,整数型变量<br>
  2.total_pageviews:总页面浏览量,整数型变量<br>
  3.edu:教育程度,分类型变量<br>
  4.edu_ages:受教育年限,整数型变量<br>
  5.user_level:用户等级,分类型变量<br>
  6.industry:用户行业划分,分类型变量<br>
  7.value_level:用户价值度分类,分类型变量<br>
  8.act_level:用户活跃度分类,分类型变量<br>
  9.sex:性别,分类型变量<br>
  10.blue_money:第一类优惠券订单金额,整数型变量<br>
  11.red_money:第二类优惠券订单金额,整数型变量<br>
  12.work_hours:工作时间长度,整数型变量<br>
  13.region:地区,分类型变量<br>
response:响应值,整数型变量,1代表用户有响应,0代表用户未响应<br>

#项目步骤:
---
1.数据加载<br>
2.数据审查与预处理<br>
3.获得最佳模型参数<br>
4.分类模型训练<br>
5.分类模型预测<br>
6.评估模型<br>

#项目主要应用技术
---
* 主要用到的库:Numpy、Pandas和Sklearn<br>
* 使用OneHotEncoder进行二值化标志转换<br>
* 使用数据降维SelectPercentile结合基于方差分析的f_classif选择最明显的特征<br>
* 使用管道方法Pipe、交叉检验cross_val_score、分层采样StratifiedKFold与集成分类算法AdaBoostClassifier获得最佳模型参数<br>

#项目文件目录
---
* market_activity.xlsx->会员活动数据集
* market_predict.ipynb->数据分析程序  

#项目运行环境
---
--------------------
* 数据分析程序需要在Anaconda2-4.2.0(64-bit)环境中运行,该环境保存程序的注释及其运行结果  
--------------------
