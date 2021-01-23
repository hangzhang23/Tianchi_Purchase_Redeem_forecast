# 天池竞赛：资金流入流出预测

这是一个天池的[长期赛](https://tianchi.aliyun.com/competition/entrance/231573/introduction)，整体从理解题意到数据到最后的模型流程完整的走一遍天池的数据比赛。

- [数据探索](https://github.com/hangzhang23/Tianchi_Purchase_Redeem_forecast/blob/main/purchase_redeem_descovery.ipynb)：分析数据以及特征的特点
- 特征工程：如果按照回归任务来说，需要更多相关的特征，所以这部分根据需求用不同的方法构建特征
- 模型构建：
  - [时间序列模型-ARIMA](https://github.com/hangzhang23/Tianchi_Purchase_Redeem_forecast/blob/main/purchase_redeem_ARMA.ipynb)
  - [时间序列模型-时序规则法](https://github.com/hangzhang23/Tianchi_Purchase_Redeem_forecast/blob/main/Purchase_Redeem_tsr.ipynb)
  - [回归模型](https://github.com/hangzhang23/Tianchi_Purchase_Redeem_forecast/blob/main/Purchase_redeem_models.ipynb)：LR，GBDTRegressor,lightGBMRegressor,GBDTRegressor,xgboostRegressor,RandomForestRegressor,DecisionTreeRegressor
  
最终得分：
- ARIMA（105）
- 时序规则法（135）
- 回归模型（LR在使用纯bool特征时为128）

最终结论是，如果把赛题按照回归任务来做，特征工程是非常耗时间并且又很考验业务能力的的一步，一旦特征工程做的好，即便使用很简单的模型都可以得到很好的效果。
