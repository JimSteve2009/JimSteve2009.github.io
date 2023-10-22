# 个人博客的搭建

博客（Blog）对于理工科研工作者来说，能够提供一个分享/交流/学习的平台，值得花一些时间来建立自己的blog。我的博客搭建方案是Github Page托管+Hugo网站生成器。搭建起来比较方便，也适合像我这种非IT专业人士。

具体搭建步骤包括，

##### 一、Hugo 生成网站： 

1）安装Hugo Extended 2）运行命令`Hugo new site`, 注意命令应在网页根目录下进行，此步将生成相应的网页文件夹 3）安装git，使用git clone命令从GitHub上下载[Hugo网页主题](https://themes.gohugo.io/)，注意下载的主题文件要放到themes文件夹下 4）将themes中的config配置文件移动到根目录，并相应修改、配置、添加网页内容，可使用`Hugo server -D`查看建立的网页情况 5）运行命令`hugo`，发布网页生成public文件。

##### 二、将Public文件夹上传到Github仓库，并启用GitHub Page：
1）注册、登录GitHub并建立仓库，在settings->pages里面启用GitHub Pages,此时会生成你的site 2）Public文件夹上传，网页经过hugo命令发布后，我们仅需要public里的文件即可发布网页。首先打开git bash，并切换到public文件夹下，依次使用命令
- `git init -b main` 
- `git remote add origin {{your Github address}}`
- `git add .`
- `git push -u origin main`

上传到GitHub库之后，等待1分钟左右，即可通过Page地址访问我们发布的网页啦:smile:。

我写的过程比较简单，具体操作过程中可能会遇到一些细节问题。可以参考网上其他详细教程，比如[小绵尾巴博客](https://cuttontail.blog/blog/create-a-wesite-using-github-pages-and-hugo/)。

 
