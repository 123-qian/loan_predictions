# loan_predictions说明

- dataset包含`account.txt`、`card.txt`、`client.txt`、`disp.txt`、`district.txt`、`loan.txt`、`order.txt`、`trans.txt`八个文件。
- `loan(satcking).ipynb`使用stacking构建模型，auc在验证集上0.82；
- `loan_lr(lgb).ipynb`分别使用logistic regression和lgb构建模型，lr得分为0.882，lgbm得分平均为0.77，最终在验证集上为0.885(数据量小，分数产生波动)；
- 特征衍生针对该类问题比较重要，数据量较大时，lgb需要进一步调参。
