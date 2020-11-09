## 项目介绍
守护者消防安全知识答题小程序

马上就119了，应景开发了一个消防知识答题闯关小程序，

## 联系方式

如需搭建消费答题小程序请联系开发者微信：xfy6369

## 本文背景
今天是该小程序正式开放运营的第一天，参与答题的用户数据，我通过控制台看了下有88人，67人完成了答题，也就是闯关成功

今日用户数据截图



数据库集合截图如下



## 闯关规则

![输入图片说明](https://images.gitee.com/uploads/images/2020/1107/142244_3117686b_1307964.png "屏幕截图.png")


## 相关问题
文章的标题为复盘所以我讲下从开发到上线运营遇到的一些问题

1）云函数异常导致订阅消息发送失败

订阅消息为云函数发送，由于今天云函数的异常导致有二条订阅消息发送失败，因为闯关成功是推送消息的，而且线下抽奖也是凭订阅消息，所以如果订阅消息发送失败，那么就导致已成功闯关，但无法抽奖。

备注：每个微信号每天只能参与答题一次

目前小程序未对发送失败进行处理，这个地方后期可迭代优化掉

该问题在社区已提问，具体帖子如下所示

云函数报错？? - 微信开放社区 https://developers.weixin.qq.com/community/develop/doc/0000a0c56189a06a6a3b2acff5b000

2）分享复活

由于目前分享之后没有成功或者失败的回调，所以在这个地方存在一些问题，由于闯关答题是有倒计时，时间限制的，所以用户分享解锁之后，倒计时的开始时间不好把握，因为我目前对分享操作的回调触发是用户弹出分享窗口就开始还是分享出去才算 开始，如下图所示





从下图的调试信息可以看到，当出现这个分享弹窗的时候，倒计时已经开始了，这不是预期的效果。



 

## 参考资料
1）小程序分享及用户信息授权等接口能力的调整通知

https://mp.weixin.qq.com/cgi-bin/announce?action=getannouncement&announce_id=11536230584k14IW&version=&lang=zh_CN&token=

2）分享功能调整

https://mp.weixin.qq.com/cgi-bin/announce?action=getannouncement&announce_id=11526372695t90Dn&version=&lang=zh_CN&token=

3）“分享监听”能力调整? - 微信开放社区 https://developers.weixin.qq.com/community/develop/doc/0000447a5b431807af57249a551408

 

## 界面截图
 

截图一
 ![输入图片说明](https://images.gitee.com/uploads/images/2020/1107/142050_08c06e67_1307964.png "屏幕截图.png")


截图二
![输入图片说明](https://images.gitee.com/uploads/images/2020/1107/142124_97d3c2a2_1307964.png "屏幕截图.png")


截图三


![输入图片说明](https://images.gitee.com/uploads/images/2020/1107/142129_46e71813_1307964.png "屏幕截图.png")
截图四

![输入图片说明](https://images.gitee.com/uploads/images/2020/1107/142134_07eaefa7_1307964.png "屏幕截图.png")

截图五

![输入图片说明](https://images.gitee.com/uploads/images/2020/1107/142140_0aa99a13_1307964.png "屏幕截图.png")

截图六

![输入图片说明](https://images.gitee.com/uploads/images/2020/1107/142147_b7b0b417_1307964.png "屏幕截图.png")

截图七

![输入图片说明](https://images.gitee.com/uploads/images/2020/1107/142154_2823f68b_1307964.png "屏幕截图.png")

截图八

## 本文总结
该小程序区别于以往我的答题小程序，在交互上更友好一些，更适合于做一些带娱乐性质的答题活动，后续小程序开发方向还有待市场检验，后面也会继续迭代一些其他功能，未来可期
