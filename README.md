
# 前言

近闲,遂决定搭建博客,览阅数篇文章,捣鼓几时 终 搭建ok(谢我司一ruby大神助力).

期间弃github.io主题极丑,遂换大神iissnan的[hexo-theme-next主题](https://github.com/iissnan/hexo-theme-next/)一个,颜值瞬间爆也~

正 项目空时 , 梳理 几篇文章 share 一下自己develop时的心得 ,装 一下平时的X.

SO,I will start my loaded technology blog tour, please begin to fasten your seat belt.
(我将开始我的装逼技术博客之旅,请旅客开始系好安全带.)

{% endcq %}


# 安装步骤

## 环境位置
[Node.js](https://nodejs.org/)

Git

[github](https://github.com/)账号(新建一个repo,注意保密协议使用MIT,项目名:你的github账号.github.io)

## 安装Hexo

sudo npm install -g hexo

装完 选个文件夹 执行:

hexo init

再装完 博客根目录就ok了; 

but,还需要生成静态页面:

hexo generate

最后启动服务:

hexo server 

浏览器进入http://localhost:4000就可以调试了!

## 引入Github
打开博客根目录的_config.yml文件,修改

     deploy:
     
     type: git

     repo: https://github.com/你的github名/你的github名.github.io.git

     branch: master

最后执行:

npm install hexo-deployer-git --save

部署:

hexo deploy

此时你就可以打开你的博客:

http://你的github名.github.io

## 总结

每次部署执行主要代码:

    hexo clean

    hexo generate

    hexo deploy

一些常用命令:


	hexo new"postName" #新建文章

	hexo new page"pageName" #新建页面

	hexo generate #生成静态页面至public目录

	hexo server #开启预览访问端口（默认端口4000，'ctrl + c'关闭server）

	hexo deploy #将.deploy目录部署到GitHub

	hexo help # 查看帮助

	hexo version #查看Hexo的版本

---
