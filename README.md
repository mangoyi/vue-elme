# vue-elme

> sell app

## Build Setup


#git clone https://github.com/mangoyi/vue-elme.git
git cone https://github.com/mangoyi/vue-elme.git

# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev



#Summary 

vue.js 高仿饿了么手机端开发 --webapp页面开发流程

```
	需求分析=>脚手架工具=>数据mock=>架构设计=>代码编写=>项目测试=>编译打包
```

#技术
```	1、vue1.0版本```
```	2、vue-resource 前后端交互```
```	3、vue-router 前端路由实现单页面```
```	4、better-scroll 第三方库```
```	5、ES6语法```
```	6、styl语法```
#vue.js介绍
	MVVM框架--针对复杂的交互逻辑应用
		   --提供基础的架构抽象
		   --通过ajax数据持久化
	vue.js 核心=>数据驱动+组件化的前端开发
	vue轻便，适合移动端开发。
#核心思想： 数据驱动
	1、曾经的前端开发：后台传输数据，前台视图需要通过手动操作DOM节点实现
	2、vue中只需要处理数据，vue通过directive对DOM进行封装，通知指令修改对应DOM（DOM是数据的一种自然映射，数据改变驱动视图自动更新）
#核心思想：组件化
	扩展HTM元素，封装可重用代码
###组件设计原则
	1、页面中每个独立的可视可交互区域视为一个组件（每个组件对应一个工程目录，组件所有资源放在该目录下就近维护）
	2、就近维护：前端工程化思想，每个开发者知道自己开发维护的功能单元，而每个功能单元包含了样式逻辑js代码等
	3、页面是组件的容器，组件可以嵌套自用组合成完整的页面

----------

#项目文件夹说明
	1、node-modules   npm install安装的依赖代码库
	2、src 目录存放源码（所有代码放在该目录）
	3、static 存放第三方静态资源
	4、.babelrc  babel编译的配置（将ES6语法转换成ES5语法）
	5、.editorconfig 编辑器的配置
	6、.eslintignore 忽略语法检查的文件
	7、.eslintrc.js eslint的配置文件（exteds:'standard' 标准规则，'rule' 修改部分规则）
	8、.gitignore 忽略部分文件不提交到git代码库
	9、index.html 入口html文件
	10、build文件和config文件 主要是webpack配置的相关文件
#项目搭建基本流程
	1、npm install -g vue-cli（vue-cli是vue脚手架工具）
	2、vue init vuejs-templates/webpack#1.0 sell (sell是项目名，#1.0代表安装vue版本)
	-----vue init webpack sell（安装最新版本，而该项目开发的vue版本是1.0，所以一定要选择#1.0版本）
	3、cd sell (进入sell文件夹)
	4、npm install （安装node-modules文件，依赖的代码库文件）
	5、npm run dev (启动server)

#常见git报错解决方案
	报错：缺少依赖stylus
	
	1、package.json中添加'stylus-loader':'^2.1.1'
	2、执行npm install (相当于npm install stylus-loader 安装stylus模块)
	3、npm install stylus
	4、npm install stylus-loader --save-dev(如果以上两个安装方式任然报错，则通过本行命令。)
	--sava-dev 表示将包安装到devDependencies，表示你开发时依赖的包

