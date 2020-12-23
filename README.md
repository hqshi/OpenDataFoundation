# OpenDataFoundation

## 便捷、客观的GTA5游戏数据查询平台
支持平台

* 微信
* 1. 微信公众号 R星速递
* 2. 微信小程序 洛圣都 Express
* Api 暂未开放
* QQ群机器人 因腾讯限制，暂时不提供支持

## 介绍页面
> #### <a href="verson update.md">规则更新日志</a>

## 已完成和关闭的项目的列表
请在以下的页面查看更多消息


> #### <a href="closed.md">暂时不会提供支持的功能</a>
> 过于占用服务器资源和理念相悖或是当前无法实现的功能
> #### <a href="finished.md">已升级的功能</a>
> 已经测试并开发了的功能
> #### <a href="stop.md">已暂停开发</a>
> 出于各种考虑取消开发的功能
## 待完成的功能

### 当前开发序列
* 小程序新使用模型
* 服务器在线状态监测(https://support.rockstargames.com/zh/servicestatus)
* 添加单项判断 




## 项目介绍
```

---
#### 功能名
**简介**:

**实现**:


```


---
#### 模块重构
**简介**:将代码进行分离

**实现**:tool文件太大了，还是分离一下吧

---
#### 数据库重构
**简介**:修改数据库结构，添加历史记录

**实现**:创建新的数据库

---
#### 使用手册
**简介**:简要的使用说明，包含各判定结果说明？

**实现**:简单介绍

---

#### 数据项详解
**简介**:解释各数据项的来源和从何而来

**实现**:字面意思，写一下构成


---

#### 小程序历史查询ID以及当前查询ID解析
**简介**:为了更方便的使用小程序，尝试以便利贴或搜索记录形式展示历史查询记录。实时显示当前输入内容的ID解析，避免玩家以为只能查自己ID的一半

**实现**:历史记录以搜索框或本地存储的形式，解析则是新建一个展示框实时更新输入ID解析

---

#### 小程序生成分享海报
**简介**:生成一个包含全部内容的分享海报

**实现**:不太清楚，可能需要改变小程序的结构以适应从海报直接跳转的功能。海报内容不定，可能是少数文字，或者是完整图表。

要求至少比公众号的文字看的全

---

#### 查看历史查询记录
**简介**:查数据时能直接查看玩家的历史数据记录

**实现**:查询后跳转至玩家个人数据页面，同时展示当前和历史数据

---

#### 历史数据检测
**简介**:根据历史记录来检测玩家短时间又没有作弊

**实现**:两次查询之间的时间，看看又没有违规

**疑问**:如何确定多个角色，是否只统计共同数据？

---

#### 登录自己的账号
**简介**:了解R星的登录计算规则，使用用户自己的账号来查询

**实现**:带参数时走登录模式

---
#### 快速查询
**简介**:优化数据库结构和查询流程，提升查询速度

**实现**:看小程序功能升级而定

