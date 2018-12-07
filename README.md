# 前端知识点 2018

> 大致基于 react 社区。

* 框架
	* 三大框架里选哪个？
		* react
		* angular
		* vue
	* 考虑小程序？
		* 用原生、vue、还是 react 语法？
		* 是否要考虑代码共用？
		* 小程序 -> vue|react 还是 vue|react -> 小程序？
* 语言
	* 引入强类型语言？
		* TypeScript
		* Flow
	* 支持的话，后面所有的流程都需要额外考虑，比如 test、构建、数据流、三方库支持等等
* CSS
	* 预编译语言选哪个？
		* less
		* sass
		* stylus
	* 如何避免命名冲突？
		* css modules
			* 如何让部分文件不使用 css modules？
		* bem
	* 考虑 css-in-js？
		* emotion
	* 主题、在线换肤？
* 数据流
	* 数据流选哪个？
		* redux
			* redux 副作用库选哪个？
				* redux-thunk
				* redux-saga
				* redux-observable
			* 要不要用 dva 或 rematch？
			* redux-persistent
		* mobx
			* 要不要上 mobx-state-tree?
		* rxjs
		* 小而美的 unstated
		* 原生的 context + hooks
* 构建工具
	* 构建工具选哪个？
		* webpack
			* 怎么配？最佳实践是啥？
			* 如何让使用者扩展 webpack 配置？
				* webpack-chain
				* webpack-merge
			* tree-shaking 是啥？怎么开？
			* svg as component
			* 如何处理 HTML 文件？要不要用 html-webpack-plugin？
			* 待补充，这里内容太多了。。
		* rollup
		* parcel
		* system-js
	* 压缩
		* JavaScript 压缩用啥？
			* uglifyjs2 - uglifyjs-webpack-plugin
			* uglify-es - terser-webpack-plugin
			* babel-preset-minify
		* CSS 压缩用啥？
			* cssnano
			* clean-css
	* babel
		* 如何选择合适的 babel preset 和插件？
		* 如何选择必要的语法特性？一些不必要的语法会引入额外的尺寸。
		* 如何选择合适的补丁方案？
			* env + targets 配置
				* 用 entry 还是 usage
			* transform-runtime + runtime
		* node_modules 要不要编译？
			* 不按规则转成 es5 再发布的 npm 包怎么处理？
				* es5-imcompatible-versions
		* 要不要用 macros？
		* 如何写插件实现定制语法修改？
	* AST
		* 用哪套方案？
			* babel 全家桶，parser + traverse + types + template + generator
			* 老牌方案，esprima + escodegen + esquery
		* 要不要考虑封装后的 jscodeshift？
	* SourceMap
	* PostCSS
		* 如何选择合适的插件？
		* autoprefixer
			* 如何保证给 babel 补丁方案的浏览器配置是同一份？
		* 是否启用高清方案？
* 组件工具
	* 文档工具用哪个？
		* docz
		* storyboard
		* vuepress
	* 打包支持 TODO
* UI 库
	* 选哪个？
		* ant-design
		* ice
* 数据通讯
	* 选哪个请求库？
		* whatwg-fetch
		* axios
	* graphql
	* websocket
	* 如何 mock 数据？
* 包管理工具
	* 包管理选哪个？
		* npm
		* yarn
			* 要不要试着开启 Plug'n'Play？
	* 访问慢怎么办？
		* 自搭源服务
		* cnpm
	* 有私有包的需求？
* 路由
* 测试
	* 测试框架选哪个？
		* jest
		* mocha + istanbul + chai | expect + sinon
	* 


