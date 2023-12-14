# ios plist文件  用于iOS安装app
> 在github 模拟一个https的url
> 每个项目的 ios 包文件上传后 ，都要配置对应的 plist 文件，用来在 safari浏览器 直接打开安装包
> plist文件命名规则，(xxx.plist) xxx 用 uni-app中 configProject.js中 各项目的appCode 替换

> app项目发布地址 http://47.122.9.74:2345/#/app/publish

> github下载 https://github.com/jacey-xu/jacey-xu.github.io.git

> plist 模板 见 iosTemp.plist
> 
> storm 拉取github 报错
> fatal: unable to access ‘XXX.git/‘: SSL certificate problem:unable to get local issuer certificate
> 这个是由于Git默认开启了SSL验证，关闭即可
> git config --global http.sslverify false
上面这行命令的影响范围是系统当前用户，如果要设置为全局所有用户，可以改成这样：
git config --system http.sslverify false