代码托管平台 https://gitlab.eduxiji.net/
一、注册用户
1、注册时会给注册邮箱发送一封确认邮件，点击Confirm your account即可跳转到登陆界面。



2、登陆成功后出现欢迎界面，由队长点击Create a group创建一个团队。（如下图所示）


团队名称命名规范：
CSC2020-学校简称-队伍名（队伍名尽量非中文，如为中文，需填入路径信息，路径只能包含字母、数字、‘-’、，无法以‘-’开头，以“.git”结尾或以“.atom”结尾），中间以‘-’隔开
团队简介：
2020系统能力培养大赛学校名称队伍名称
可见等级设为Private
示例如下图：


3、添加组员（注意设置权限，只有Developer及以上权限才能新建分支创建合并请求等）




4、在新建的组中创建一个名为compiler的仓库作为开发仓库
注：可见等级设为Private







二、开发完成后即可提交进行测评
提交内容：
提交文件命名为project.gitpro，文件内容为私有仓库地址（需加上Doploy token）

提交文件project.gitpro生成步骤：
1.web端打开仓库，选择Settings->Repository


2.展开Deploy Tokens



3.填写过期时间等信息（只能包含字母、数字、‘-’、，无法以‘-’开头）

4.点击Create deploy token生成，然后将生成的信息复制出来备用。

5.复制出项目地址

6.将生成的Doploy token加入Clone with HTTPS链接即为完整的仓库地址
6.1添加规则（此处的username是生成Doploy token处的账号密码）：
https://<username>:<deploy_token>@gitlab.example.com/tanuki/awesome_project.git
6.2 提交内容完整示例如下：
https://abc:jDkP7VM92Zs7cGMGmn8x@gitlab.eduxiji.net/csc2020-buaa-xxx/compiler.git

7.新建project.gitpro文件，将上一步生成的仓库地址写入project.gitpro文件中，如图：





进入作业提交，选择文件，找到project.gitpro文件，点击提交


提交完成
确认提交完成之后，回到web gitlab页面下Deploy Tokens，撤销令牌使token失效
