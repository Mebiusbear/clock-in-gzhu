# 广州大学GZHU健康打卡

## 简介

1. 脚本使用Github Actions进行健康打卡
2. 脚本将在北京时间07点30分自动运行
3. 脚本支持自动上游同步更新

## 使用教程

### 必要设置

首先Fork本项目并进入Fork的项目中

然后创建两个[Repository secrets](https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository)

- 第一个Secret的Name为XUHAO，注意XUHAO要大写
- Value为学号

---

- 第二个Secret的Name为MIMA，注意MIMA要大写
- Value是密码

最后开启[workflow](https://docs.github.com/en/actions/managing-workflow-runs/disabling-and-enabling-a-workflow#enabling-a-workflow)，workflow有两个：一个打卡，一个上游同步

### 推送打卡成功与否的消息（可选功能）

#### pushplus 推送加 微信公众号

- 额外创建一个[Repository secret](https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository)
- Secret的Name为PUSHPLUS，注意PUSHPLUS要大写
- Value为pushplus 推送加 的token

## FAQ

### Q: 脚本运行失败怎么办？

如果你是第一次运行脚本，请先检查学号密码是否输入错误

## License

Copyright (c) LihaoLikeOrangeJuice. All rights reserved.

Licensed under the [MIT](LICENSE) license.
