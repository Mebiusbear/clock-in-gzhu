# 广州大学GZHU健康打卡

## 简介

1. 脚本使用Github Actions进行健康打卡
2. 脚本将在北京时间07点30分自动运行
3. 脚本支持自动上游同步更新

## 使用教程

### 必要设置

创建两个Repository secrets（在Settings中的Actions secrets里）

- 第一个Secret的Name为XUHAO，注意XUHAO要大写
- Value为学号

---

- 第二个Secret的Name为MIMA，注意MIMA要大写
- Value是密码

### 推送打卡成功与否的消息（可选功能）

#### pushplus 推送加 微信公众号

- 额外创建一个Repository secret（在Settings中的Actions secrets里）
- Secret的Name为PUSHPLUS，注意PUSHPLUS要大写
- Value为pushplus 推送加 的token

## FAQ

### Q: 脚本运行失败怎么办？

如果你是第一次运行脚本，请先检查学号密码是否输入错误

## License

Copyright (c) LihaoLikeOrangeJuice. All rights reserved.

Licensed under the [MIT](LICENSE) license.
