最近几天一直在开发一个答题闯关小程序，目前该小程序已正式发布，收到很好的运营效果

本文背景

我个人做答题小程序有一段时间了，陆陆续续出过刷题小程序、考研答题小程序、成语答题小程序，党建答题小程序，截止今天我可以说产品系列可以新增一成语：闯关答题小程序

小程序目前已发布上线，由于各方面都还需要时间不断迭代完善，暂定该版本为v1.0

本文内容

本文主要简单介绍目前闯关答题小程序实现的功能

1）小程序首页
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201102200814229.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NzM5NTY5NA==,size_16,color_FFFFFF,t_70#pic_center)


2）答题

3）活动规则介绍页
![在这里插入图片描述](https://img-blog.csdnimg.cn/2020110220083019.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NzM5NTY5NA==,size_16,color_FFFFFF,t_70#pic_center)


4）奖励介绍页

![在这里插入图片描述](https://img-blog.csdnimg.cn/20201102200842692.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NzM5NTY5NA==,size_16,color_FFFFFF,t_70#pic_center)

5）错题展示页
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201102200850881.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NzM5NTY5NA==,size_16,color_FFFFFF,t_70#pic_center)


6）排名页
![在这里插入图片描述](https://img-blog.csdnimg.cn/20201102200835727.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NzM5NTY5NA==,size_16,color_FFFFFF,t_70#pic_center)


作为一个常规的答题活动小程序具有首页、答题、排名、活动规则介绍页之外，该小程序的特殊之处在于新增了分享复活这个逻辑

由于目前分享已不能获得是否成功还是失败的回调，所以只要发起分享，便认为是一次成功的分享，获取一次复活卡

界面截图

小程序首页
![输入图片说明](https://images.gitee.com/uploads/images/2020/1102/201201_2578019e_1307964.png "屏幕截图.png")





截图二


[图片上传中…(image-8Kt7iUqqquBVXPY0nkYY)]



截图三


![输入图片说明](https://images.gitee.com/uploads/images/2020/1102/201145_1418f030_1307964.png "屏幕截图.png")



截图四

![输入图片说明](https://images.gitee.com/uploads/images/2020/1102/201150_b7287730_1307964.png "屏幕截图.png")




截图五


[图片上传中…(image-a4AQjNuLrIHenr4kIOy2)]



截图五

![输入图片说明](https://images.gitee.com/uploads/images/2020/1102/201201_346f7820_1307964.png "屏幕截图.png")




参考资料

1）小程序分享及用户信息授权等接口能力的调整通知

https://mp.weixin.qq.com/cgi-bin/announce?action=getannouncement&announce_id=11536230584k14IW&version=&lang=zh_CN&token=

2）分享功能调整

https://mp.weixin.qq.com/cgi-bin/announce?action=getannouncement&announce_id=11526372695t90Dn&version=&lang=zh_CN&token=

本文总结

本文主要分享了一个闯关答题小程序，目前该小程序已发布上线，后续会随着用户的使用反馈，进行版本的不断迭代升级