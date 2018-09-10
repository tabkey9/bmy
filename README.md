## 简介

```html
        #######################################################################
        ################                           		###############
        ################   项目方向：博客园/平台   		###############
        ################   项目名称：斑马缘        		 ###############
        ################   官网：http://miniblog.top 	      ##################
        ################                          		###############
        #######################################################################
        
	MiniBlog是一个迷你博客园(平台)，由“zebra”（斑马）开发小组共同完成以及维护的实例项目。
	我们的服务宗旨是：提供免费的入驻博客园服务，享受免费的博文发布以及博文管理服务！MiniBlog欢迎您的入驻！
	成员名单：@TabKey9、柯小花、王小贱、冰镇可乐、油条和豆浆；
```
演示：[斑马缘](https://miniblog.top)



## install
```php
# 历史源码：直接从 GitHub 上克隆即可获得；

# Git install 
git clone https://github.com/tabkey9/bmy.git
# Or
git clone git@github.com:tabkey9/bmy.git

# SVN install
svn export svn://不愿暴露IP/ --username 不愿暴露用户名 --password 不愿暴露密码 --no-auth-cache  --force
# 开源时间：2018-04-12！

# MySQL 
导入根目录下“zebra.sql”文件，记得删除SQL文件！

# TP3 MySQL配置
\Application\Common\Conf\config.php

return array(
	//'配置项'=>'配置值'
	// 模板布局
	'LAYOUT_ON'=>true,
	'LAYOUT_NAME'=>'layout',
	//数据库配置信息
	'DB_TYPE'   => 'mysql', // 数据库类型
	'DB_HOST'   => 'localhost', // 服务器地址
	'DB_NAME'   => 'zebra', // 数据库名
	'DB_USER'   => 'root', // 用户名
	'DB_PWD'    => 'root', // 密码
	'DB_PORT'   => 3306, // 端口
	'DB_PREFIX' => 'zebra_', // 数据库表前缀 
	'DB_CHARSET'=> 'utf8', // 字符集
);

# 有疑问请来信：当前页面的底部有联系方式。
```



## 开发环境参考

`预定开发环境选择(LNMP)：Linux/CentOS6.8.32+Nginx/Stableversion1.12.2 +MySQL+PHP/5.6.34`

## 已知问题汇总：
问：为什么我 git clone 之后访问出现链接已重置的提示？怎么办？

答：我也尝试了一下，确实如此。

解决方案：你根据实际情况完善一下数据库配置文件“\Application\Common\Conf\config.php”，然后删除TP框架自动生成的Runtime目录，你再访问首页试试。我这边验证过了，可行的。

问：我也想参与开发，为什么不能合并分支？

答：感谢你的贡献，但是请你在本地执行这个指令忽略掉数据库配置文件，再请求合并主分支。

```
git update-index --assume-unchanged Application/Common/Conf/config.php
```

## 联系我们

Email: admin@tlip.cn