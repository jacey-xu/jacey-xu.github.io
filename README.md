# ios plist文件  用于iOS安装app
> 在github 模拟一个https的url
> 每个项目的 ios 包文件上传后 ，都要配置对应的 plist 文件，用来在 safari浏览器 直接打开安装包
> plist文件命名规则，(xxx.plist) xxx 用 uni-app中 configProject.js中 各项目的appCode 替换

> app项目发布地址 http://47.122.9.74:2345/#/app/publish

> github下载 https://github.com/jacey-xu/jacey-xu.github.io.git

> plist 模板 见 iosTemp.plist
> 

# storm
* storm 配置关联Git（github和Gitee）并导入项目到远程仓库（Github、Gitee）
``` 原文链接：https://blog.csdn.net/m0_46378271/article/details/125921108
2.1 关联git.exe
    打开Idea左上角的Settings，选择我们上一步安装的bin下git.exe
2.2 关联 GitHub 上的账户
    选择Settings–>Github–>＋–>Log in to Github，登录Github账号
2.22 配置Github的用户名和邮箱【这一步要在上传之前配置好，否则会出现上传失败只传了仓库名的问题，且删除仓库名之后一直出重名的bug，解决起来很麻烦！！！】
    注意标红区域，提示我们还需要配置一下用户名以及邮箱：
    打开git bash，输入如下代码：这里选择自己的Github用户名和邮箱
git config --global user.name "xhy"  //用户名配置
git config --global user.email "xhy@qq"  //邮箱地址配置

————————————————
```
* storm 拉取github 报错
> fatal: unable to access ‘XXX.git/‘: SSL certificate problem:unable to get local issuer certificate
> 这个是由于Git默认开启了SSL验证，关闭即可
> git config --global http.sslverify false
上面这行命令的影响范围是系统当前用户，如果要设置为全局所有用户，可以改成这样：
git config --system http.sslverify false (无权限)