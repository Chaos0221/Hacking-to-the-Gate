# 目录
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [React](#react)
    - [创建组件的三种方式及区别](#%E5%88%9B%E5%BB%BA%E7%BB%84%E4%BB%B6%E7%9A%84%E4%B8%89%E7%A7%8D%E6%96%B9%E5%BC%8F%E5%8F%8A%E5%8C%BA%E5%88%AB)
    - [常用的 React 生命周期函数](#%E5%B8%B8%E7%94%A8%E7%9A%84-react-%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F%E5%87%BD%E6%95%B0)
    - [React 17 和现版本的区别](#react-17-%E5%92%8C%E7%8E%B0%E7%89%88%E6%9C%AC%E7%9A%84%E5%8C%BA%E5%88%AB)
    - [React 创建更新的方式](#react-%E5%88%9B%E5%BB%BA%E6%9B%B4%E6%96%B0%E7%9A%84%E6%96%B9%E5%BC%8F)
    - [React fiber](#react-fiber)
    - [React Hooks](#react-hooks)
    - [React 缺点](#react-%E7%BC%BA%E7%82%B9)
    - [React 性能优化](#react-%E6%80%A7%E8%83%BD%E4%BC%98%E5%8C%96)
    - [Redux 特点](#redux-%E7%89%B9%E7%82%B9)
    - [Redux 缺点](#redux-%E7%BC%BA%E7%82%B9)
    - [PureComponent 和 Component 区别](#purecomponent-%E5%92%8C-component-%E5%8C%BA%E5%88%AB)
    - [高阶组件是什么](#%E9%AB%98%E9%98%B6%E7%BB%84%E4%BB%B6%E6%98%AF%E4%BB%80%E4%B9%88)
    - [Provider 如何实现将全局store传递给后代组件？connect 具体如何实现？](#provider-%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%E5%B0%86%E5%85%A8%E5%B1%80store%E4%BC%A0%E9%80%92%E7%BB%99%E5%90%8E%E4%BB%A3%E7%BB%84%E4%BB%B6connect-%E5%85%B7%E4%BD%93%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0)
- [JavaScript](#javascript)
    - [cookie 和 WebStorage 的相同点和区别](#cookie-%E5%92%8C-webstorage-%E7%9A%84%E7%9B%B8%E5%90%8C%E7%82%B9%E5%92%8C%E5%8C%BA%E5%88%AB)
    - [数组去重方法](#%E6%95%B0%E7%BB%84%E5%8E%BB%E9%87%8D%E6%96%B9%E6%B3%95)
    - [如何理解闭包？闭包有什么优缺点？](#%E5%A6%82%E4%BD%95%E7%90%86%E8%A7%A3%E9%97%AD%E5%8C%85%E9%97%AD%E5%8C%85%E6%9C%89%E4%BB%80%E4%B9%88%E4%BC%98%E7%BC%BA%E7%82%B9)
    - [ES6 新特性](#es6-%E6%96%B0%E7%89%B9%E6%80%A7)
    - [ES7 ES8 新特性](#es7-es8-%E6%96%B0%E7%89%B9%E6%80%A7)
    - [ES9 新特性](#es9-%E6%96%B0%E7%89%B9%E6%80%A7)
    - [ES10 新特性](#es10-%E6%96%B0%E7%89%B9%E6%80%A7)
    - [继承的几种方式](#%E7%BB%A7%E6%89%BF%E7%9A%84%E5%87%A0%E7%A7%8D%E6%96%B9%E5%BC%8F)
    - [new 具体做了什么？](#new-%E5%85%B7%E4%BD%93%E5%81%9A%E4%BA%86%E4%BB%80%E4%B9%88)
    - [如何实现深拷贝？](#%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%E6%B7%B1%E6%8B%B7%E8%B4%9D)
    - [如何实现浅拷贝](#%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%E6%B5%85%E6%8B%B7%E8%B4%9D)
    - [普通函数和箭头函数的区别](#%E6%99%AE%E9%80%9A%E5%87%BD%E6%95%B0%E5%92%8C%E7%AE%AD%E5%A4%B4%E5%87%BD%E6%95%B0%E7%9A%84%E5%8C%BA%E5%88%AB)
    - [设计模式](#%E8%AE%BE%E8%AE%A1%E6%A8%A1%E5%BC%8F)
    - [什么是面向对象](#%E4%BB%80%E4%B9%88%E6%98%AF%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1)
    - [什么是调用栈](#%E4%BB%80%E4%B9%88%E6%98%AF%E8%B0%83%E7%94%A8%E6%A0%88)
- [移动端](#%E7%A7%BB%E5%8A%A8%E7%AB%AF)
    - [如何实现移动端响应式布局](#%E5%A6%82%E4%BD%95%E5%AE%9E%E7%8E%B0%E7%A7%BB%E5%8A%A8%E7%AB%AF%E5%93%8D%E5%BA%94%E5%BC%8F%E5%B8%83%E5%B1%80)
    - [1px边框问题](#1px%E8%BE%B9%E6%A1%86%E9%97%AE%E9%A2%98)
    - [适配刘海屏](#%E9%80%82%E9%85%8D%E5%88%98%E6%B5%B7%E5%B1%8F)
- [HTML](#html)
    - [HTML5 新特性](#html5-%E6%96%B0%E7%89%B9%E6%80%A7)
- [CSS](#css)
    - [CSS3 新特性](#css3-%E6%96%B0%E7%89%B9%E6%80%A7)
    - [如何让一个不定宽高的元素水平垂直居中](#%E5%A6%82%E4%BD%95%E8%AE%A9%E4%B8%80%E4%B8%AA%E4%B8%8D%E5%AE%9A%E5%AE%BD%E9%AB%98%E7%9A%84%E5%85%83%E7%B4%A0%E6%B0%B4%E5%B9%B3%E5%9E%82%E7%9B%B4%E5%B1%85%E4%B8%AD)
    - [flex弹性盒模型](#flex%E5%BC%B9%E6%80%A7%E7%9B%92%E6%A8%A1%E5%9E%8B)
- [浏览器](#%E6%B5%8F%E8%A7%88%E5%99%A8)
    - [前端如何SEO (搜索引擎优化)](#%E5%89%8D%E7%AB%AF%E5%A6%82%E4%BD%95seo-%E6%90%9C%E7%B4%A2%E5%BC%95%E6%93%8E%E4%BC%98%E5%8C%96)
    - [从输入URL到页面显示的过程发生了什么？](#%E4%BB%8E%E8%BE%93%E5%85%A5url%E5%88%B0%E9%A1%B5%E9%9D%A2%E6%98%BE%E7%A4%BA%E7%9A%84%E8%BF%87%E7%A8%8B%E5%8F%91%E7%94%9F%E4%BA%86%E4%BB%80%E4%B9%88)
    - [如何优化WEB性能时间？](#%E5%A6%82%E4%BD%95%E4%BC%98%E5%8C%96web%E6%80%A7%E8%83%BD%E6%97%B6%E9%97%B4)
    - [HTTPS和HTTP的区别](#https%E5%92%8Chttp%E7%9A%84%E5%8C%BA%E5%88%AB)
    - [三次握手和四次挥手](#%E4%B8%89%E6%AC%A1%E6%8F%A1%E6%89%8B%E5%92%8C%E5%9B%9B%E6%AC%A1%E6%8C%A5%E6%89%8B)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


# React 

### 创建组件的三种方式及区别

1. 无状态函数式组件/ 静态组件

    - 只有传入的 props 属性，没有 this/ state/ 生命周期方法
    - 组件不会被实例化，提升渲染性能

2. 有状态组件 
    
    - 实例化，有 this/ state/ 生命周期方法

    - React.createClass（ES5声明的类组件）
        - 自动绑定函数方法的 this 指向，导致不必要的性能开销
        - mixins 不够自然

    - class App extends React.Component（ES6声明的类组件）
        - 只绑定需要用 this 的函数，提升性能
        - mixins 适合高阶组件


### 常用的 React 生命周期函数

1. render 
    渲染组件 创建虚拟DOM

2. componentDidMount componentDidUpdate 
    能获取真实DOM 一般做ajax操作

3. shouldComponentUpdate 
    判断更新前后的state或props是否相同 如果相同就return false 不更新


### React 17 和现版本的区别

1. 移除三个生命周期方法 

    - componentWillMount 
    - componentWillReceiveProps 
    - componentWillUpdate 

2. 引入两个生命周期函数

(1) getDerivedStateFromProps
    - 静态方法 无法使用 this；
    - 根据传入的 props 来更新 state；
    - 返回修改后的 state 如果不修改 返回 null。

(2) getSnapshotBeforeUpdate
    - 在更新阶段的render后调用；
    - 返回值作为第三个参数传给 componentDidUpdate。

### React 创建更新的方式
- ReactDOM.render / hydrate
    - 创建 ReactRoot
    - 创建 FiberRoot RootFiber
    - 创建更新
- setState
- forceUpdate


### React fiber
- 每个React.creatElement 对应一个fiber对象
- 记录节点的各种状态（fiber更新后才会更新类组件的state props）
- 串联整个应用形成树结构（从fiberRoot开始遍历节点的子节点 遇到叶子节点return 找它的父节点的兄弟节点 继续遍历子节点 直到return到fiberRoot结束）

### React Hooks
- 16.8新增
- 解决的问题：Provider 高阶组件等抽象层组件会形成嵌套地狱; 类组件中一个逻辑被分割在多个生命周期中
- useState useEffect等API使无状态组件有状态 实现状态逻辑的复用
- const [state, setState]=useState(defaultState)
- useEffect(()=>{副作用操作}) 每次更新都调用    


### React 缺点
- 只关注视图 数据管理过于复杂 需要安装大量第三方库来方便开发

### React 性能优化
- 减少在render中创建变量和bind
- PureComponent immutable
- 重写shouldComponentUpdate
- reselect


### Redux 特点
- 单一数据源（所有状态都存储在全局store）
- 只读状态（只有通过dispatch(action)修改状态）
- 用纯函数修改状态 保持状态稳定性

### Redux 缺点
- 数据流复杂 需要维护大量的action reducer等
- 默认不支持异步操作 需要安装中间件

### PureComponent 和 Component 区别

- React.Component 并未实现 shouldComponentUpdate()，而 React.PureComponent 中以浅层对比 prop 和 state 的方式来实现了该函数。

- 如果对象中包含复杂的数据结构，则有可能因为无法检查深层的差别，产生错误的比对结果。仅在你的 props 和 state 较为简单时，才使用 React.PureComponent，或者在深层数据结构发生变化时调用 forceUpdate() 来确保组件被正确地更新。你也可以考虑使用 immutable 对象加速嵌套数据的比较。

### 高阶组件是什么
- 高阶组件是参数为组件，返回值为新组件的函数。
- 常用的高阶组件：withRouter(传递match history location) connect AntD的form.create


### Provider 如何实现将全局store传递给后代组件？connect 具体如何实现？
- 父组件使用 getChildContext()，将 store 放到它的 context 里面；子组件可以通过 contextTypes 来声明想要的 context 里面的哪些状态，然后通过 this.context 访问到那些状态。
- connect 通过接受 mapStateToProps 和 mapDispatchProps 参数，将 context 中的数据取出来，并以 prop 的形式传递给组件。





# JavaScript

### cookie 和 WebStorage 的相同点和区别

1. 相同点: 
    - 保存在浏览器
    - 只有同源网址能访问

2. 不同点:
    - 存储容量不同
        - cookie 4K
        - WebStorage 5M

    - 每次http请求 cookie会随请求头一起发给服务器
        WebStorage不会

    - 生命周期不同
        - cookie: 如果设置过期时间 到过期时间销毁; 如果没设置 浏览器关闭销毁
        - sessionStorage: 浏览器窗口关闭则销毁
        - localStorage: 永久保存 手动删除才销毁

    - 作用域不同
        - sessionStorage不在不同窗口中共享
        - localStorage和cookie在同源窗口中共享 


### 数组去重方法

1. 用ES6新增数据结构Set 
    - let newArr=[...new Set(arr)]
    - 将数组元素添加到Set中 重复项不会被添加进去 

2. 用indexOf方法
    - 新建空数组 遍历原数组
    - 用indexOf在空数组中查找数组项 
    - 如果返回-1 则将这一项添加进空数组

3. 用indexOf方法
    - 新建空数组 遍历原数组
    - 用indexOf在原数组中查找数组项 
    - 如果返回值和数组项的索引相同 则将这一项添加进空数组


### 如何理解闭包？闭包有什么优缺点？

- 闭包是能访问函数内局部变量的私有函数

- 优点:
    - 能突破作用域 通过统一接口访问局部变量
    - 减少声明全局变量 避免污染顶级作用域

- 缺点: 
    变量无法被垃圾回收机制回收 滥用闭包容易造成内存泄漏
    解决方法：在使用完闭包后将它赋值为 null



### ES6 新特性
- let const 
- 箭头函数
- 类 继承
- promise
- generator iterator
- 扩展运算符
- 字符串模板
- for-of 遍历
- Map Set
- module import export
- proxy
- Symbol
- 新增string number Math的API



### ES7 ES8 新特性

- ES7
    - 求幂运算符 **
    - 数组方法 includes() 查看数组是否有某元素 返回布尔值 

- ES8
    - async await 
    - Object.values()
    - Object.entries()
    - padStart() padEnd() 字符串补全方法

### ES9 新特性

- 在同步循环中写异步函数 await for-of async
- Promise.finally()
- rest/spread 

### ES10 新特性
[尝鲜 ES2019 的新功能](https://juejin.im/post/5c8a14ba5188251bde6be098)

1. flat(depth) 扁平数组

2. flatmap(value=>{}) 扁平并遍历数组

3. Object.fromEntries() 根据键值对生成对象

4. trimStart()/ trimLeft(); trimeEnd()/ trimRight() 删除字符串前面 or 后面的空格   

5. try-catch结构中 catch可以不写变量


### 继承的几种方式
1. 原型链
- 将父类的实例作为子类的原型
- Son.prototype = new Father();

2. 原型拷贝
- for-in 将父类原型上的键值拷贝到子类原型上

3. 构造器
- 复制父类的实例属性给子类
- 在子类中 Father.call()

4. 组合
- 构造器拷贝属性+原型拷贝方法

5. 对象冒充
- 在子类中this.father=Father; this.father(name)



### new 具体做了什么？
1. 创建一个空对象 
2. 这个空对象的__proto__指向构造器的prototype
3. 调用构造器函数 函数内this指向这个新对象
4. 如果构造函数return了一个对象，那么这个对象会取代new出来的对象。如果构造函数没有return对象，那么返回这个新对象


### 如何实现深拷贝？
1. JSON.stringify JSON.parse
2. 封装函数 对于对象类型的键值递归拷贝 对基本类型的键值直接return

### 如何实现浅拷贝
1. Object.assign()
2. 拓展运算符
3. 封装函数（for-in遍历原对象 把属性值对添加进新对象中）

### 普通函数和箭头函数的区别

1. 箭头函数捕获声明时的上下文环境作为this指向 普通函数式this指向调用它的对象
2. 无法用 call bind apply 改变箭头函数的this指向
3. 箭头函数没有arguments 用rest参数代替
4. 箭头函数没有prototype 不能当做构造器函数


### 设计模式

1. 工厂模式
- 将new操作单独封装

2. 观察者模式
- 发布 & 订阅
- 一个对象状态变化 可以通知多个观察者
场景：
- 事件监听
- promise
- nodejs中 events 自定义事件
- React Vue中组件生命周期
- Vue的watch

3. 装饰者模式
- 给对象或类添加新功能 不改变其原有的结构和功能（如手机壳）
- 场景：ES7装饰器语法 (balbel-plugin-transform-decorators-legacy 在类前一行写@装饰器函数名)

4. 代理模式
- 使用者通过代理对象访问目标对象
场景
- ES6 Proxy
    let prx=new Proxy(obj, {
        get(target, key){
            ...
            return target[key]
        },
        set(target, key, val){
            ...
            target[key]=val
        }
    })
- jQuery 
    $.proxy(函数, this) 绑定this指向

5. 迭代器模式
- 顺序访问一个有序集合
- 使用者无需知道内部结构（封装）
- ES6的iterator: Array Map Set String arguments 等数据结构的prorotype上都有[Synbol.iterator]属性 属性值是函数 执行函数返回迭代器 有next方法顺序迭代子元素


### 什么是面向对象
意义：数据结构化
1. 继承
- 子类继承父类
- 可以复用公共方法，减少冗余
2. 封装
- 数据的权限和保密 
- 减少耦合 
- public 完全开放(默认), protected 对子类开放, private 只对自己开放（不包括实例对象）
- TS支持 ES6一般不支持 用_属性名来表示私有属性 
3. 多态
- 同一接口的不同实现
- 面向接口编程
- 保持子类的灵活性

### 什么是调用栈

调用栈是一种解析器去处理程序的机制，它是栈数据结构。它能追踪子程序的运行状态。

- 函数被调用时，会被添加到调用栈中
- 任何在这个函数内部调用的函数，会被添加到调用栈中
- 当执行完这个函数后，如果它没有调用其他函数，则它会从调用栈中推出。
- 异步函数的回调函数一般都会被添加到运行队列里面，如settimeout会在响应的时间后把回调函数放入队列中，队列里的函数需要等栈为空时才会被推入栈中执行。如果队列中有其他函数，需要等队列前面的函数被堆入调用栈中之后才会运行。



# 移动端

### 如何实现移动端响应式布局

1. rem+js
    - 让html的font-size响应式变化
    - 长度单位用rem的元素也随之变化

2. flex+vw vh
    - 给父元素设置display:flex 子元素设置flex值 实现等比例分割
    - 长度单位用vw vh 实现响应式变化

3. flexible
    - 原理：将html的font-size设置成布局viewport的1/10; 根据dpr设置body的font-size
    - 使用方式：1. 在模板文件或在入口文件中引入lib-flexible包 实现响应式 2. 配置loader或插件 将css文件中的px自动转换为rem值 简化开发
    - 配置方式：
    在react-webpack环境中：下载px2rem-loader并在webpack.config.js中配置
    在dva环境中：下载postcss-pxtorem插件 将.webpackrc改成.webpackrc.js 配置插件
    在vue环境中：下载pxtorem-loader 在build文件夹的utils中配置


### 1px边框问题
[移动端适配(掘金)](https://juejin.im/post/5cddf289f265da038f77696c#heading-21)

问题：在设备像素比大于1的屏幕上，我们写的1px实际上是被多个物理像素渲染，这就会出现1px在有些屏幕上看起来很粗的现象

解决方案：
1. border-image
    .border_1px{
        border-bottom: 1px solid #000;
    }
    @media only screen and (-webkit-min-device-pixel-ratio:2){
        .border_1px{
            border-bottom: none;
            border-width: 0 0 1px 0;
            border-image: url(../img/1pxline.png) 0 0 2 0 stretch;
        }
    }

2. background-image
    .border_1px{
        border-bottom: 1px solid #000;
    }
    @media only screen and (-webkit-min-device-pixel-ratio:2){
        .border_1px{
            background: url(../img/1pxline.png) repeat-x left bottom;
            background-size: 100% 1px;
        }
    }

3. 伪类+transform
    .border_1px:before{
        content: '';
        position: absolute;
        top: 0;
        height: 1px;
        width: 100%;
        background-color: #000;
        transform-origin: 50% 0%;
    }
    @media only screen and (-webkit-min-device-pixel-ratio:2){
        .border_1px:before{
            transform: scaleY(0.5);
        }
    }
    @media only screen and (-webkit-min-device-pixel-ratio:3){
        .border_1px:before{
            transform: scaleY(0.33);
        }
    }

4. svg
PostCSS的postcss-write-svg我们能直接使用border-image和background-image创建svg的1px边框

5. 设置viewport (早期flexible的解决方案)
    通过设置缩放，让CSS像素等于真正的物理像素。
    例如：当设备像素比为3时，我们将页面缩放1/3倍，这时1px等于一个真正的屏幕像素。

### 适配刘海屏
刘海屏无法显示的区域：圆角（corners）、刘海（sensor housing）和小黑条（Home Indicator）。
安全区域是不受上面三个效果的可视窗口范围。

1. 设置meta标签
content='viewport-fit=contain/auto'

2. 使用IOS11新增CSS函数 env constant
body {
  padding-bottom: constant(safe-area-inset-bottom);
  padding-bottom: env(safe-area-inset-bottom);
}
    

# HTML

### HTML5 新特性

- 更简洁的文档声明 <!DOCTYPE>

- 新增API
    - 离线存储 webStorage
    - file API
    - 重力感应 调用摄像头 麦克风

- 新增语义化标记
    header footer section nav aside canvas audio video 

- 新增属性
    - 表单标记属性: placeholder autocomplete
    - 全局属性: hidden data-自定义属性





# CSS

### CSS3 新特性

- 新增选择器
    - 结构化伪类: first-child last-child nth-child only-child
    - 状态伪类: enabled disabled checked等
    - 伪元素: after before not

- 新增样式
    - flex 弹性盒模型
    - 媒体查询 实现响应式布局
    - 服务器端字体 图标字体 @font-face{}
    - transform 变形 (translate scale rotate)
    - transition 过渡
    - content 内容 一般和伪元素配合使用
    - animation 实现动画
    - 圆角边框 border-radius
    - 背景样式 background-size

### 如何让一个不定宽高的元素水平垂直居中

1. 父元素display: flex; justify-content: center; align-items: center
2. 父元素position:relative
    子元素position:absolute; left:50%;top:50%; transform: translate(-50%, -50%)
3. 父元素position: relative; 子元素position:absolute; left,right,top,bottom: 0; margin: auto
4. 如果是图片 可以将它设置为父元素的背景图片 background: url() no-repeat center;

### flex弹性盒模型
https://www.cnblogs.com/qingchunshiguang/p/8011103.html
http://www.ruanyifeng.com/blog/2015/07/flex-examples.html
采用display: flex的元素称为flex容器，容器存在两根主轴：水平方向的主轴 (main axis) 和垂直方向的交叉轴 (cross axis)。容器中子元素默认按主轴排列。
弹性盒模型主要适用于应用程序的组件及小规模布局（栅格布局针对大规模布局）
1. 容器属性
主轴方向 flex-direction: row/ row-reverse/ column/ column-reverse	
是否换行 flex-wrap: no-wrap/ wrap/ wrap-reverse
在主轴上的对齐方式 justify-content: flex-start/ flex-end/ center/ space-between/ space-around
在交叉轴上的对齐方式 align-items: stretch/ flex-start/ flex-end/ center/ baseline
多轴的对齐方式 align-content: stretch/ flex-start/ flex-end/ center/ baseline
2. 子元素属性
排列顺序 order: 整数
放大比例 flex-grow: 数字
缩小比例 flex-shrink: 非负整数
再分配多余空间前项目占据的主轴空间 flex-basis: auto/ px
flex: flex-grow flex-shrink flex-basis 的缩写（后两个可选）
3. 当容器设置display: flex 时，子元素设置以下属性不会生效
a)	float
b)	clear 
c)	vertical-align
d)	column




# 浏览器

### 前端如何SEO (搜索引擎优化)

1. 合理的title、description、keywords
    - 搜索对着三项的权重逐个减小
    - title值强调重点即可，重要关键词出现不要超过2次，而且要靠前，不同页面title要有所不同
    - description把页面内容高度概括，长度合适，不可过分堆砌关键词，不同页面description有所不同
    - keywords列举出重要关键词即可

2. 语义化的HTML代码，符合W3C规范

3. 重要内容HTML代码放在最前
    - 搜索引擎抓取HTML顺序是从上到下，有的搜索引擎对抓取长度有限制，保证重要内容一定会被抓取

4. 重要内容不要用js输出：
    - 爬虫不会执行js获取内容

5. 少用iframe：
    - 搜索引擎不会抓取iframe中的内容

6. 非装饰性图片必须加alt

7. 提高网站速度
    - 网站速度是搜索引擎排序的一个重要指标


### 从输入URL到页面显示的过程发生了什么？

1. 查看浏览器缓存 如果有 直接从缓存中读取
2. DNS解析域名
3. 浏览器向服务器发起TCP连接 进行三次TCP握手
4. 握手成功后 浏览器向服务器发送HTTP请求和请求数据
5. 服务器处理请求 把响应数据（网页资源）发给浏览器
6. 浏览器读取响应数据 解析HTML源码 生成DOM树 解析CSS JS


### 如何优化WEB性能时间？

1. 尽量减小网页资源体积
    - JS CSS代码压缩
    - 优化图片
    - 代码纯手写

2. 减少HTTP请求次数
    - JS CSS代码合并 模块化开发
    - CSS Sprites
    - Webpack配置loader 将较小图片打包进JS文件

3. 异步加载JS
    - 操作DOM的JS用defer
    - 不操作DOM的JS用async

4. CSS代码优化
    - 按渲染顺序写选择器
    - 后代选择器不超过三层
    - 颜色不缩写
    - 样式初始化
    - 不用通用选择器

5. JS代码优化
    - React Vue用虚拟DOM和diff算法减少DOM刷新
    - 原生JS用文档碎片
    - 用if-else代替if-else if
    - 避免死循环
    - 少用闭包


### HTTPS和HTTP的区别

1、https需要ca申请证书，需要交费。

2、http是明文传输的超文本传输协议，https用ssl加密的传输协议。

3、端口不同。http是80，https是443。

4、http的连接是无状态的；HTTPS协议是由SSL+HTTP协议构建的可进行加密传输、身份认证的网络协议，比http协议安全。

5. HTTPS协议握手阶段比较费时，会使页面的加载时间延长近50%，增加10%到20%的耗电

6. 采用HTTPS加密的网站在搜索结果中的排名将会更高



### 三次握手和四次挥手

三次握手：TCP连接时客户端和服务端要互相确认 共发送三个包（由客户端connect()开始）
1. 客户端发送SYN 进入SYN_SEND状态
2. 服务器发送SYN+ACK 进入SYN_RECV状态
3. 客户端发送ACK 双方均进入ESTABLISH状态

四次挥手：TCP断开连接前互相确认
1. 客户端发送FIN 关闭数据传送 进入FIN-WAIT状态
2. 服务器发送ACK 进入CLOSE-WAIT状态
3. 服务器关闭连接 发送FIN 进入LAST-ACK状态
4. 客户端发送ACK 进入TIME-WAIT状态 服务器接收到后双方进入CLOSED状态
