# 广州大学GZHU健康打卡

## 简介

脚本使用Github Actions进行健康打卡  
将在北京时间07点30分自动运行  
支持自动上游同步更新  
支持pushplus 推送加 推送消息

## 使用教程

### 必要设置

1. Fork本项目并进入Fork的项目中
2. 创建两个[Repository secrets](https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository "教程")，如下表

|Secret|Name|Value|
|-|-|-|
|1|XUHAO|学号|
|2|MIMA|密码|

3. 开启[Workflows](https://docs.github.com/en/actions/managing-workflow-runs/disabling-and-enabling-a-workflow#enabling-a-workflow "教程")，有两个Workflows：一个打卡，一个上游同步

### 推送打卡成功与否的消息（可选功能）

#### pushplus 推送加 微信公众号

额外创建一个[Repository secret](https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository "教程")

|Secret|Name|Value|
|-|-|-|
|1|PUSHPLUS|pushplus 推送加 的Token|

## FAQ

### Q: 脚本运行失败怎么办？

如果你是第一次运行脚本，请先检查学号密码是否输入错误

## License

Copyright (c) LihaoLikeOrangeJuice. All rights reserved.

Licensed under the [MIT](LICENSE) license.
