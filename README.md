# QCAFE

## startup 程序运行入口
支持修改参数：
1. 数据集路径
2. 数据集选择
3. batchsize
4. 学习率lr
5. 训练epoch数

## run 运行调用文件
### run 运行调用统一入口
### init 导入本文件夹内所有定制函数
### run_cafe 运行调用模型
支持修改参数：
1. 数据集文件名
2. 优化器
3. 训练入口 trainer.fit
4. 测试入口
新增：
1. 学习率调度
2. 预训练参数加载
3. 模式选择：train/test

## train 训练步骤文件
### trainer 训练通用步骤
### cafe_trainer 模型训练具体步骤
train_epoch结果打印

## model 模型文件
### model 抽象模型
### cafe
### QAttention3 原网络
### QA 新网络

## tb-logs
使用命令：tensorboard --logdir=tb_logs/
查看训练数据图像