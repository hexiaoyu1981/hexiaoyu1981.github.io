# 一个用GitHub Pages构建极简博客的例子

为完全没有编程基础的朋友准备的，尽可能简化，以便画瓢。包括：

* 包含动态分类目录和静态链接（About, Contact）的首页`index.html`；
* 预制示例用的`favicon.ico`文件、静态文件`about.md, contact.md`、博客帖子；
* 预制的配置文件`_config.yaml`，能适应官方内置的模板；

部署地址[在此](http://blog.xiiigame.com/GitHubPagesBlogExample/)。

## 安装要点

* 建立一个远程公开库
  * 库名使用`你的github用户名.github.io`的是用户主站；否则是项目站点，将自动放置于`你的github用户名.github.io/库名`。
  * `Source`选`master branch`
* 克隆本库到本地，并与远程库关联
  * `_config.yml`中已经为你把`theme`设置为`Minimal theme`

请参考[官方完善的入门教程](https://guides.github.com/features/pages/)。

## 博客写作要点

* 要写的博客放在`_posts`内，编码一律用UTF-8（无头信息）；
* 文件名格式为`YYYY-MM-DD-filename.md`，前三段是年月日；
* 帖子需要有YAML头信息才能在站内由Jekyll转换成html文件。请看[Jekyll的YAML头信息参考](http://jekyllcn.com/docs/frontmatter/)。
  * `tags`在当前模板、首页中暂时没用，可以不填；
  * `date`信息将覆盖文件名中的时间信息，格式为`YYYY-MM-DD HH:MM:SS +/-TTTT`，时分秒和时区可以省略；
* 使用Markdown语法写博客。请看[Markdown语文参考](https://guides.github.com/features/mastering-markdown/)。

若想深入学习，请看[jekyllcn.com](http://jekyllcn.com/)。

## VSCode操作要点

建议用VSCode来写作，同时用它来管理GitHub库。
VSCode的Git History插件能使Git操作变得更直观。

* 通过左侧的源码控制工具栏，把修改commit/提交到本地库；
* 通过左下状态栏的同步按钮，同步本地库与远程库；

也能在GitHub上直接修改，但请记得及时同步，以免两头同时修改一个文件而导致导致冲突。
**一旦出现冲突，如果不熟悉git操作，请务必做好备份后再处理。**
