# 切题类
1.要求自我介绍  
2.介绍最近一年内比较有成就感的项目，其中完成最有难度的部分有哪些？  
3.开发的项目内容主要有哪些  
4.最近正在学习的技术或内容
# HTML类
### 1.**HTML5有哪些新特性、移除了那些元素？如何处理HTML5新标签的浏览器兼容问题？如何区分 HTML 和HTML5？**
A：HTML5 现在已经不是 SGML 的子集，主要是关于图像，位置，存储，多任务等功能的增加。  
**新增的特性**  
绘画 canvas、用于媒介回放的 video 和 audio 元素、本地离线存储 localStorage 长期存储数据，浏览器关闭后数据不丢失；sessionStorage 的数据在浏览器关闭后自动删除；语意化更好的内容元素，比如 article、footer、header、nav、section；表单控件，calendar、date、time、email、url、search；新的技术webworker, websockt, Geolocation  
**移除的元素**  
纯表现的元素：basefont，big，center，font, s，strike，tt，u；  
对可用性产生负面影响的元素：frame，frameset，noframes；  
**支持HTML5新标签兼容处理**  
IE8/IE7/IE6支持通过document.createElement方法产生的标签，  
可以利用这一特性让这些浏览器支持HTML5新标签，  
浏览器支持新标签后，还需要添加标签默认的样式：  
**区分方式**  
通过文档头进行区分，H5为
### 2.**cookies，session，sessionStorage 和 localStorage的区别**
cookie在浏览器和服务器间来回传递。 sessionStorage和localStorage不会  
sessionStorage和localStorage的存储空间更大；  
sessionStorage和localStorage有更多丰富易用的接口；  
sessionStorage和localStorage各自独立的存储空间；
# CSS类
### 1.CSS实现垂直水平居中
position+margin/tranfrom  table flex inline  
参考链接：[http://www.codeceo.com/article/css-vertical-6-ways.html](http://www.codeceo.com/article/css-vertical-6-ways.html)
### 2.css选择符及其排序
import 内联元素 #id 》class=属性 》元素=伪元素  
[http://www.cnblogs.com/zxjwlh/p/6213239.html](http://www.cnblogs.com/zxjwlh/p/6213239.html)
### 3.两栏等高布局、三栏等高布局写法以及原理
float、position、flex、table  
[http://www.cnblogs.com/lyzg/p/5164593.html](http://www.cnblogs.com/lyzg/p/5164593.html)  
[http://www.cnblogs.com/lyzg/p/5160570.html](http://www.cnblogs.com/lyzg/p/5160570.html)
### 4.说明盒子模型，以及兼容使用盒子模型
### 5.display、position、float互相的影响
[http://blog.csdn.net/baoxiaofeicsdn/article/details/58603959](http://blog.csdn.net/baoxiaofeicsdn/article/details/58603959)
### 6.BFC（margin 塌陷、清除浮动）
块级格式化上下文  
[http://www.cnblogs.com/lhb25/p/inside-block-formatting-ontext.html](http://www.cnblogs.com/lhb25/p/inside-block-formatting-ontext.html)
### 7.CSS3新特性（flex、calculate）
[https://www.ibm.com/developerworks/cn/web/1202\_zhouxiang\_css3/](https://www.ibm.com/developerworks/cn/web/1202_zhouxiang_css3/)
### 8.CSS3动画（translate、transform、animation、keyframes）
[http://www.w3cplus.com/content/css3-animation](http://www.w3cplus.com/content/css3-animation)  
[http://blog.bingo929.com/transform-translate3d-translatez-transition-gpu-hardware-acceleration.html](http://blog.bingo929.com/transform-translate3d-translatez-transition-gpu-hardware-acceleration.html)
### 9.清除浮动
额外标签法、使用:after 伪元素、给父元素定高、利用overflow:hidden;属性、父元素浮动、父元素处于绝对定位  
[https://segmentfault.com/a/1190000003937063](https://segmentfault.com/a/1190000003937063)
### 10.flex 兼容问题
[https://segmentfault.com/a/1190000003978624#articleHeader8](https://segmentfault.com/a/1190000003978624#articleHeader8)
# JS类
### 1.特殊值与运算符
### 2.ES6基本概念和语法
### 3.js类的继承的几种方式优缺点
ES6类继承是基于prototype，是语法糖
### 4.模块化的实现？
### 5.事件轮询？事件模型？任务轮询？异步（js引擎的异步原理）
### 6.网站攻击的方式
xss（富文本不能转义）、csrf、的了解和产生？
### 7.事件监听，冒泡和捕获。
### 8.jsbridge的实现原理
### 9.跨域
jsonp、代理服务
http://www.cnblogs.com/jesseZh/p/4921494.html
10.前端路由实现方式
HTML5 History两个新增的API：history.pushState 和 history.replaceState，两个 API 都会操作浏览器的历史记录，而不会引起页面的刷新。
Hash就是url 中看到 # ,我们需要一个根据监听哈希变化触发的事件( hashchange) 事件。我们用 window.location 处理哈希的改变时不会重新渲染页面，而是当作新页面加到历史记录中，这样我们跳转页面就可以在 hashchange 事件中注册 ajax 从而改变页面内容。 可以为hash的改变添加监听事件：
```
window
.addEventListener(
"hashchange"
, funcRef, 
false
)
```
* 优点

从性能和用户体验的层面来比较的话，后端路由每次访问一个新页面的时候都要向服务器发送请求，然后服务器再响应请求，这个过程肯定会有延迟。而前端路由在访问一个新页面的时候仅仅是变换了一下路径而已，没有了网络延迟，对于用户体验来说会有相当大的提升。
前端路由的优点有很多，比如页面持久性，像大部分音乐网站，你都可以在播放歌曲的同时，跳转到别的页面而音乐没有中断，再比如前后端彻底分离。 开发一个前端路由，主要考虑到页面的可插拔、页面的生命周期、内存管理等。
* 缺点

使用浏览器的前进，后退键的时候会重新发送请求，没有合理地利用缓存。
History interface提供了两个新的方法：`pushState()`,`replaceState()`使得我们可以对浏览器历史记录栈进行修改：
# 兼容性类
1.移动端web的兼容性bug  
1、一些情况下对非可点击元素如(label,span)监听click事件，ios下不会触发，css增加cursor:pointer就搞定了。  
2.position 在Safari下的两个定位需要都写，只写一个容易发生错乱  
3.Input 的placeholder会出现文本位置偏上的情况  
input 的placeholder会出现文本位置偏上的情况：PC端设置line-height等于height能够对齐，而移动端仍然是偏上，解决是设置line-height：normal  
4.zepto点击穿透问题  
引入fastclick解决；event.preventDefault  
5.当输入框在最底部的时候，弹起的虚拟键盘会把输入框挡住。

Element.scrollIntoViewIfNeeded(opt\_center)
# node类
[http://www.admin10000.com/document/6715.html](http://www.admin10000.com/document/6715.html)  

[https://github.com/jimuyouyou/node-interview-questions](https://github.com/jimuyouyou/node-interview-questions)

**node**的构架
 异步错误捕获
**node**有哪些定时功能?
 setTimeout/clearTimeout, setInterval/clearInterval, setImmediate/clearImmediate, process.nextTick
 
 事件循环是什么样子的?  
参考答案: event loop其实就是一个事件队列，先加入先执行，执行完一次队列，再次循环遍历看有没有新事件加入队列．执行中的叫IO events, setImmediate是在当前队列立即执行,setTimout/setInterval是把执行定时到下一个队列，process.nextTick是在当前执行完，下次遍历前执行．所以总体顺序是: IO events >> setImmediate >> setTimeout/setInterval >> process.nextTick

# 框架类
## react基本原理
### 1.dom diff原理
2.setState实现原理
setState —》 batchUpdate —>transaction
### 3.bind的方式
4.组件生命周期
dom diff？setState？bind（this）？
### 5.react组件性能优化
使用PureRenderMixin、shouldComponentUpdate来避免不必要的虚拟DOM diff，在render内部优化虚拟DOM的diff速度，以及让diff结果最小化。
## Vue基本原理
### 1.MVVM
model+view+viewModel框架，数据模型model，viewModel连接两个。数据操作比较多的场景，更加便捷
### 2.双向数据绑定
vue.js 是采用数据劫持结合发布者-订阅者模式的方式，通过`Object.defineProperty()`来劫持各个属性的`setter`，`getter`，在数据变动时发布消息给订阅者，触发相应的监听回调。  
**具体步骤：**  
**第一步：需要observe的数据对象进行递归遍历**，包括子属性对象的属性，都加上`setter`和`getter`  
这样的话，给这个对象的某个值赋值，就会触发`setter`，那么就能监听到了数据变化  
**第二步：compile解析模板指令**，将模板中的变量替换成数据，然后初始化渲染页面视图，并将每个指令对应的节点绑定更新函数，添加监听数据的订阅者，一旦数据有变动，收到通知，更新视图  
**第三步：Watcher订阅者是Observer和Compile之间通信的桥梁**，主要做的事情是:  
1、在自身实例化时往属性订阅器(dep)里面添加自己  
2、自身必须有一个update()方法  
3、待属性变动dep.notice()通知时，能调用自身的update()方法，并触发Compile中绑定的回调，则功成身退。  
**第四步：MVVM作为数据绑定的入口，整合Observer、Compile和Watcher三者**，通过Observer来监听自己的model数据变化，通过Compile来解析编译模板指令，最终利用Watcher搭起Observer和Compile之间的通信桥梁，达到数据变化 -> 视图更新；视图交互变化(input) -> 数据model变更的双向绑定效果。
### 3.vuejs生命周期
总共分为8个阶段创建前/后，载入前/后，更新前/后，销毁前/后。  
**创建前/后：**在beforeCreated阶段，vue实例的挂载元素$el和数据对象data都为undefined，还未初始化。在created阶段，vue实例的数据对象data有了，$el还没有。  
**载入前/后：**在beforeMount阶段，vue实例的$el和data都初始化了，但还是挂载之前为虚拟的dom节点，data.message还未替换。在mounted阶段，vue实例挂载完成，data.message成功渲染。  
**更新前/后：**当data变化时，会触发beforeUpdate和updated方法。  
**销毁前/后：**在执行destroy方法后，对data的改变不会再触发周期函数，说明此时vue实例已经解除了事件监听以及和dom的绑定，但是dom结构依然存在
### 4.**vuex是什么**
vue框架中状态管理。通过状态（数据源）集中管理驱动组件的变化（好比spring的IOC容器对bean进行集中管理）。  
应用级的状态集中放在store中； 改变状态的方式是提交mutations，这是个同步的事物； 异步逻辑应该封装在action中。
### 5.vue中如何防止xss的
{{}}
{{{ options.content }}} 对于3重花括号的模板，Vue.js会将其中的HTML标签按照正常内容渲染。
### 6.父子组件如何通信  如果不是父子组件怎么通信
父传子方法
 属性传递 props、广播事件传递 vm.$broadcast 
子传父方法 
派遣事件传递 vm.$dispatch   
 兄弟组件互传
父组件代理传递 子(vm.dispatch ）父 ( vm.broadcast )子 事件方法传递
### 7.Vue 定义data的注意事项，实例是否可更改data内容
### 8.vue的nexttick实现
http://www.cnblogs.com/hity-tt/p/6729118.html
## 其他
### 1.react和vue的区别
相同点：
* 都支持服务端渲染
* 都有Virtual DOM，组件化开发，通过props参数进行父子组件数据的传递，都实现webComponents规范
* 数据驱动视图
* 都有支持native的方案，React的React native，Vue的weex

不同点：
* React严格上只针对MVC的view层，Vue则是MVVM模式
* virtual DOM 不一样 vue会跟踪每一个组件的依赖关系，不需要重新渲染整个组件树。而对于React而言，每当应用的状态被改变时，全部子组件都会重新渲染。当然，这可以通过shouldComponentUpdate这个生命周期方法来进行控制，
* 组件写法不一样 React 推荐的做法是 JSX + inline style，也就是把 HTML 和 CSS 全都写进 JavaScript 了，即”all in js” Vue 推荐的是使用`webpack + vue-loader`的单文件组件格式，即html,css,js写在同一个文件；
* 数据绑定：Vue有实现了双向数据绑定，React数据流动是单向的
* state对象在react应用中是不可变的，需要使用setState方法更新状态；在Vue中，state对象并不是必须的，数据由data属性在Vue对象中进行管理。

# 算法类
### 1.基本排序方式
冒泡、快排
### 2.算法题
回流字符串、去重等  
[https://github.com/gitWhatever/javascipt-Programming-for-interview](https://github.com/gitWhatever/javascipt-Programming-for-interview)
# 基本知识类
## 网络
### 1.get、post的区别
### 2.http状态码及其含义
### 3.ping是什么，基于什么协议
### 4.浏览器缓存cache（304、200 form cache）
### 5.输入url到显示页面的整个过程
### 6.常用的请求头信息，分为哪几块？
## 浏览器
### 1.**常见的浏览器内核？H5内核？**
Trident内核：IE,MaxThon,TT,The World,360,搜狗浏览器等。[又称MSHTML]  
Gecko内核：Netscape6及以上版本，FF,MozillaSuite/SeaMonkey等  
Presto内核：Opera7及以上。      [Opera内核原为：Presto，现为：Blink;]  
Webkit内核：Safari,Chrome等。   [ Chrome的：Blink（WebKit的分支）]
### 2.兼容性问题？
### 3.页面渲染的过程（dom树构建到用户可见）
### 4.重绘重排？（移动端和pc端的区别、滚动的时候重绘重排）
### 5.移动端的页面该如何调试？
## 其他
### 1.webpack和gulp的区别
webpack是一种模块化打包工具，主要用于模块化方案，预编译模块的方案；gulp是工具链、构建工具，可以配合各种插件做js压缩，css压缩，less编译 替代手工实现自动化工作。  
Grunt/Gulp更多的是一种工作流；提供集成所有服务的一站式平台； gulp可以用来优化前端工作流程。  
2.
# 扩展类
### 1.前端页面性能优化
[http://www.cnblogs.com/lei2007/archive/2013/08/16/3262897.html](http://www.cnblogs.com/lei2007/archive/2013/08/16/3262897.html)
