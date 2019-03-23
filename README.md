# Vue.cli3.x创建项目

**安装Vue-cli3.x的前置条件：Node.js** 

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

               旧版本卸载命令 `npm uninstall vue-cli -g `
               
                补充：vue-cli 3.x 卸载命令  `npm uninstall @vue/cli -g`    (如果需要可使用)
                ![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue450.png)

                
国内下载npm镜像速度比较慢

按需可切换为淘宝镜像，命令如下：

`npm config set registry http://registry.npm.taobao.org/`

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue612.png)

等待安装完毕

## 2.创建项目

**建议先考虑项目文件夹储存的位置并进入相关位置**，以桌面为例  `cd desktop`  如果无需更改位置，请跳过本操作

_如果需返回上级目录  cd.. 即可，其他cmd命令可自行百度_

### 2.1创建项目的两种方式：

#### 2.1.1 使用命令行创建

创建命令： vue create 项目名   **项目名自己起即可，但请注意不能有大写字母，否则报错：Warning: name can no longer contain capital letters**

`vue create learn`  √

接下来会问你选择那种配置（会显示所有保存过的配置，首次使用只会显示 default（babel,eslint） 以及 Manually select features）

可选自己之前创建过的或选择官方默认配置或者手动选择
![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue964.png)

选择Manually select features 将出现以下内容 _操控提示：方向键 控制上下 空格选择   A 全选 I反转选择_

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1001.png)

选择好大体的功能/插件之后 回车 接着会让你选择细分的特性

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1084.png)

比如 Linter/Formatter 下：

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1097.png)
 
在保存时进行代码检测

Babel、PostCSS、ESLint等配置文件存放位置，选择单独保存在各自的配置文件中

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1147.png)

Pick a CSS pre-processor(css预处理语言)下 有SCSS/SASS、LASS、Stylus

还有TS、PWA、Roter（vue 路由管理；SPA必带）、Vuex（vue状态管理）、测试（Unit Testing、E2E Testing）等等，均可按需选择

最后会询问你 是否保存为未来项目的预设配置  如果保存需要输入名称

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1325.png)
                

等待项目创建...

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1337png)

项目创建好后按提示进入项目，并启动项目

cd learn 进入后 `npm run serve`

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1386.png)

_这两个地址均可访问，第二个地址也并不能对外访问，应该是没做好端口映射，那这个地址用来干嘛的？_

#### 2.1.2通过GUI创建

在下载好vue-cli3.x后，进入项目存储位置后  输入 vue ui，会在浏览器内打开vue项目仪表盘（非初次使用界面）

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1506.png)

在使用过GUI创建过项目后，再次打开就会直接进入旧项目管理界面，如上

如果需要再新建一个项目，可在 左上角下拉菜单内选择 ”Vue项目管理器“返回首页

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1584.png)
![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1586.png)
![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1588.png)

创建——》在此创建新项目——》输入项目文件夹名（没有git建议关闭）——》下一步

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1631.png)

可选自己创建过的配置或者官方配置或者手动配置

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1632.png)

手动配置如下图所示，  按需选择，相关介绍之前提到过了

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1685.png)

_注：有下拉框的得先选择否则不能 下一步_

最后点击创建并等待

最终和CMD截图如下

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1728.png)

如果想在浏览器内启动的话 左侧菜单栏——》任务——》任务面板——》serve——》运行——》右侧 启动app  (从左往右点击红色即可)

![Image](https://github.com/l1045490877x/Learning/blob/Vue/Vue.files/Vue1799.png)

也可命令行启动，命令与之前所述相同

至此就开启了新的旅途-Vue之旅！