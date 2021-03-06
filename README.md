# weiyi114-
基于Java Web的Jiho汽车导购系统的设计与实现
# 基于Java Web的Jiho汽车导购系统的设计与实现


#### 介绍
汽车导购系统用作MyEclipse作为开发工具，整套系统采用MVC框架，逻辑操作采用JAVA进行编写，页面技术主要使用JSP，使用的数据库是MySQL，然后系统完成以后对系统进行测试，进而完善系统功能，最终完成了该系统的开发。汽车导购系统包括汽车导购信息查询，汽车订单，汽车论坛公告等几大模块。汽车导购查询可以对汽车的价格，型号，简介等信息进行查询。汽车订单模块中，可以对购买的订单进行管理，包括查询，修改等。在汽车论坛公告模块中，可以发布汽车信息，用户也可以发表自己的看法。
在相对于比较廉价的网络资源使得汽车导购系统成本低、传播广、效益高，给商家带来了无比宽广的市场，也给消费者带来了廉价优惠的汽车和更好的需求。本系统操作界面简介精美，用户体验感非常强，操作容易上手。系统更也加容易的去维护和进行升级。




#### 项目说明
汽车导购系统业务对象分为用户和汽车导购系统两个部分。图是完成整个导购过程的业务流程图，包括：登录，查看汽车分类，查看汽车的具体信息，加入购物车，支付，查看订单信息，安全退出登录等。而其他一些功能，比如后台的管理功能，用户查看站内论坛，修改个人信息等功能，则没包括在业务流程中。
![输入图片说明](https://images.gitee.com/uploads/images/2021/0126/231316_1aacfdf2_8587779.png "屏幕截图.png")

本系统含有用户与管理员两种角色，用户与管理员的功能不同，因此需要绘制两种不同的功能用例图，用户含有的功能有注册，登录，信息搜索，首页，汽车分类，汽车论坛，站内咨询，留言板，关于我们，购物车，我的订单，个人信息管理，密码修改几个功能，管理员含有的功能有会员管理，用户管理，咨询管理，友情链接，滚动图片，关于我们，汽车论坛管理，车辆类别，车辆品牌，车辆管理，车辆库存，订单管理，留言管理几个功能。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0126/231348_7001d174_8587779.png "屏幕截图.png")

本系统使用Java语言进行开发。Java是一种跨平台的语言，具有通用性，高效性，平台移植性和安全性。面向对象的三大特征分别为封装、继承和多态。
本系统使用Struts作为系统的整体基础架构，主要负责MVC的分离，在Struts框架的模型部分是负责控制业务跳转，利用Spring做管理，管理struts。具体做法是：用面向对象的分析方法根据需求提出一些模型，将这些模型实现为基本的Java对象，然后编写基本的DAO(Data Access Objects)接口，并给出DAO实现，采用DAO类来实现Java类与数据库之间的转换和访问，最后由Spring做管理，管理Struts。
系统的基本业务流程是： 在表示层中，首先通过JSP页面实现交互界面，负责接收请求(Request)和传送响应(Response)，然后Struts根据配置文件(struts-config.xml)将ActionServlet接收到的Request委派给相应的Action处理。在业务层中，管理服务组件的Spring IoC容器负责向Action提供业务模型(Model)组件和该组件的协作对象数据处理(DAO)组件完成业务逻辑，并提供事务处理、缓冲池等容器组件以提升系统性能和保证数据的完整性。
采用上述开发模型，不仅实现了视图、控制器与模型的彻底分离，而且还实现了业务逻辑层与持久层的分离。这样无论前端如何变化，模型层只需很少的改动，并且数据库的变化也不会对前端有所影响。

![输入图片说明](https://images.gitee.com/uploads/images/2021/0126/231407_d7698055_8587779.png "屏幕截图.png")

根据需求调研结果确定本系统主要包括两个大模块，分别是管理员和用户。用户功能包括注册登录，信息搜索，汽车分类查看，留言，站内资讯查看，汽车论坛的查看，我的订单，购物车，个人信息管理，以及个人密码的修改等功能。管理员功能主要包括 会员的管理，汽车类别管理，汽车品牌管理，库存管理，订单管理，留言管理，论坛管理，滚动图片的管理，站内资讯的管理等。

#### 项目截图
![输入图片说明](https://images.gitee.com/uploads/images/2021/0126/231426_4c80b5f5_8587779.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2021/0126/231433_efff34e3_8587779.png "屏幕截图.png")
![输入图片说明](https://images.gitee.com/uploads/images/2021/0126/231441_fa988494_8587779.png "屏幕截图.png")



#### 求助热线


代码有任何问题可联系
联系Q：2762501186

                            
![输入图片说明](https://images.gitee.com/uploads/images/2020/1119/003728_cd598bb9_4865385.jpeg "微信.jpg")           

感谢Github！！  
觉得项目不错的给个Star谢谢大佬！！！
提供无偿review服务
