# Vue.cli3.x创建项目

安装Vue-cli3.x的前置条件：Node.js 

以Windows为例安装Node.js,百度 “Node.js官网” 或”Node.js中文网”均可 ,如无特殊要求 下载安装 LTS版（长期支持版，该版本已满足Vue CLI官网所需要求版本要求）

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue137.png)

一路Next即可，一般无需更改默认安装设置
        
安装完毕在开始菜单内即可找到一个名为 Node.js 的文件夹如下图
        
<br/>
![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue196.png)<br>

_注：Node.js内可直接运行js基础代码（非DOM等相关代码）_

而我们需要使用的是 `Node.js command prompt`

## 1.Vue-CLI安装：

官方命令 `npm install -g @vue/cli`   

_注：@不能少，少了@安装的不是3.x版本而是1.x、2.x版本，若已经安装了旧版本则需卸载旧版本然后再安装新版本_ 

               **旧版本卸载命令 `npm uninstall vue-cli -g `** 
               
                _补充：vue-cli 3.x 卸载命令  `npm uninstall @vue/cli -g`    (如果需要可使用)_
                
国内下载速度比较慢

查看npm当前下载镜像，命令如下：

`npm get registry `

结果> https://registry.npmjs.org/

如果嫌弃下载慢可以切换为淘宝镜像，命令如下：

`npm config set registry http://registry.npm.taobao.org/`

等待安装完毕

2创建项目，但是建议先考虑项目文件夹储存的位置并进入相关位置，以桌面为例

`cd desktop`

如果无需更改位置，请跳过；如果需返回上级目录  cd.. 即可，其他cmd命令可自行百度

创建项目的两种方式：

①直接命令行创建

创建项目命令： vue create 项目名   自己起个名字即可，但请注意不能有大写字母，否则报错：Warning: name can no longer contain capital letters

`vue create learn`  √

接下来会问你选择那种配置（会显示所有保存过的配置，首次使用只会显示 default（babel,eslint） 以及 Manually select features）

可选自己之前创建过的或选择官方默认配置或者手动选择

选择Manually select features 将出现以下内容

方向键 控制上下 空格选择   A 全选 I反转选择

选择好大体的功能/插件之后 回车 接着会让你选择细分的特性

比如 Linter/Formatter 下：
 
在保存时进行代码检测

                Babel、PostCSS、ESLint等配置文件存放位置，选择单独保存在各自的配置文件中
                Pick a CSS pre-processor(css预处理语言)下 有SCSS/SASS、LASS、Stylus
                还有TS、PWA、Roter（vue 路由管理；SPA必带）、Vuex（vue状态管理）、测试（Unit Testing、E2E Testing）等等，均可按需选择
                最后会询问你 是否保存为未来项目的预设配置  如果保存需要输入名称

等待项目创建...

项目创建好后按提示进入项目，并启动项目

cd learn 进入后 `npm run serve`

这两个地址均可访问，第二个地址也并不能对外访问，应该是没做好端口映射，那这个地址用来干嘛的？

通过GUI创建

在下载好vue-cli3.x后，进入项目存储位置后  输入 vue ui，会在浏览器内打开vue项目仪表盘（非初次使用界面）

在使用过GUI创建过项目后，再次打开就会直接进入旧项目管理界面，如上

如果需要再新建一个项目，可在 左上角下拉菜单内选择 ”Vue项目管理器“返回首页

创建——》在此创建新项目——》输入项目文件夹名（没有git建议关闭）——》下一步

可选自己创建过的配置或者官方配置或者手动配置

手动配置如下图所示，  按需选择，相关介绍之前提到过了

注：有下拉框的得先选择否则不能 下一步

最后点击创建并等待

最终和CMD截图如下

如果想在浏览器内启动的话 左侧菜单栏——》任务——》任务面板——》serve——》运行——》右侧 启动app  (从左往右点击红色即可)

也可命令行启动，命令与之前所述相同

至此结束





You can use the [editor on GitHub](https://github.com/l1045490877x/Learning/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for


Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](Learning/Vue.files/Vue1001.png)
```

For more details see [GitHub Flavored Markdown]().

### Jekyll Themes
![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1001.png)

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/l1045490877x/Learning/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
