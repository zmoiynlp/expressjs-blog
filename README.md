expressjs-blog
==============

##用expressjs开发的个人博客系统

###1.安装mongodb
    sudo apt-get install mongo
###2.执行以下四条命令
    mongo
    use blog
    db.addUser("root","1234")
    db.auth("root","1234");

###3.配置 common/config.js文件
    dbName 为 blog
    dbUser 为 root
    dbPass 为 1234
    dbAddress 为 mongodb所在机器IP
注mongodb默认不能远程连接，如果需要远程连接，要更改mongo的配置。如果在本机连接，dbUser, dbPass不要填。
###4.执行
    npm install
    node server.js
###5.到 /register 下注册
注册成功之后注释掉useRoutes.js的63-66行。
###6.到 /admin下管理博客
##作者个人博客
[www.thinkspring.cn](http://www.thinkspring.cn)
