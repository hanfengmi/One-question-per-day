## 收集到的面试题

### CSS
1. 怎么实现三栏布局？ ✅       

圣杯布局、双飞翼布局、定位、flex等。。。 

[code](https://github.com/hanfengmi/One-question-per-day/blob/master/1-1%20threeColumn.html)

***
2. 垂直居中怎么做
    display:flex;
    justify-content: center;
    align-item:center;

    position:relative
    item {
        position:absolute;
        left:50%;
        top:50%;
        height:30%;
        width:50%;
        margin:-15% 0 0 -25%;
    }

    position:relative
    item {
        position:absolute;
        left:50%;
        top:50%;
        transform:translate(-50% -50%);
    }


3. 盒模型
IE: 怪异盒模型 margin+content(border+padding+text)
W3C : margin+border+padding+content

4. css单位
px vh % em cm mm

5. css选择器

**基本选择器**
*通配符
ID选择器
CLASS选择器
标签选择器
**组合选择器**
a,b a和b元素
a b a里面的选择器
a + b 紧邻a后面的b选择器
a > b a所有子元素b
**属性选择器**
a['checked']
a['val = attr'] a所有val属性等于attr的标签
a['val ^= attr'] a attr开头的
a['val $= attr'] a attr结尾的

**选择伪类**
a:first-child()
a:hover
a:focus
a:brfore
a:after

**结构性伪类**
a:nth-child(n) 匹配a的第n个元素
a:nth-last-child(n) 匹配a的倒数第n个元素
a:nth-of-type(n) 只匹配同种元素

6. 层叠上下文
层叠上下文，简单的理解，就是元素所在的一个牢笼。如果创建了这个牢笼，那它本身和它的子元素都处于这个牢笼下。
定位不是static，或者opacity不为1都会创建一个层叠上下文

7. 常见页面布局？响应式布局？


8. BFC
块状格式化上下文，

根元素或包含根元素的元素
float属性不为none;
position为absolute或fixed
display为inline-block, table-cell, table-caption, flex, inline-flex
overflow不为visible( hidden,scroll,auto, )

块格式化上下文对浮动定位与清除浮动都很重要

9. css预处理器

less scss
嵌套语法  使用变量   mixin（直接在目标位置混入另一个类样式 、 定义一个不输出的样式片段）

10. css3新特性
Word-wrap & Text-overflow
Gradient 渐变
shadow
transition trnasform animation

11. 相邻的两个inline-block节点为什么会出现间隔，该如何解决
书写习惯

inline写在一行
font-size：0后font-size：14px
margin负值
letter-spacing负值

12. meta viewport 移动端适配

js设置根字节，css使用rem+媒体查询

13. CSS实现宽度自适应100%，宽高16:9的比例的矩形
父级设置padding-bottom:56.25%

14. rem 布局的优缺点
 

15. 画三角形

border
transform

16. 1px 边框问题
scaleY(0.2)

### JS

1. 数据类型的分类和判断
**基本数据类型**
String Nuber Null Undefind Boolean
**引用数据类型**
Object Array Function
**ES6**
symbol 表示独一无二的值

typeof 只能判断string number boolean symbol undefind 
instanceof 不能判断空数组
toString 处对象需用.call [object String]

2. 原型、原型链、继承、构造函数、实例


3. 有几种方式可以实现继承，用原型实现继承有什么缺点，解决办法

4. 作用域、作用域链、闭包

5. arguments 对象

6. Ajax的原生写法

7. 对象深拷贝、浅拷贝

8. 图片懒加载、预加载

9. 实现页面加载进度条

10. this关键字

11. 函数式编程

12. 手动实现parseInt

13. 为什么会有同源策略

14. 怎么判断两个对象是否相等

15. 事件模型（事件委托、代理，如何让事件先冒泡后捕获）

16. window 的 onload 事件和 domcontentloaded

17. for...in 迭代和 for...of 有什么区别

18. 函数柯里化

19. call apply区别，原生实现bind
> call，apply，bind 三者用法和区别：角度可为参数、绑定规则（显示绑定和强绑定），运行效率、运行情况。

21. async/await

22. 立即执行函数和使用场景

23. 设计模式(要求说出如何实现,应用,优缺点)/单例模式实现

24. iframe的缺点有哪些

25. 数组问题
> 数组去重，数组常用方法，查找数组重复项，扁平化数组，按数组中各项和特定值差值排序

26. BOM属性对象方法

27. 服务端渲染

28. 垃圾回收机制

29. eventloop，进程和线程，任务队列

30. 如何快速让字符串变成已千为精度的数字

### ES6
1. let、const 声明

2. 解构赋值

3. 声明类与继承：class、extend

4. Promise 的使用与实现（原理）

5. generator（异步编程、yield、next()、await 、async）

6. 箭头函数 this 指向问题、拓展运算符

7. module

8. map 和 set 怎么用，如何实现一个数组去重，map数据结构有什么优点？

9. ES6 怎么编译成 ES5，css-loader 原理,过程

10. ES6 转成 ES5 的常见例子

11. 使用 es5 实现 es6 的 class

### 浏览器
1. 输入url到展示页面过程发生了什么？

2. 重绘与回流

3. 防抖与节流

4. cookies、session、sessionStorage、localStorage

5. 浏览器内核

### 服务端和网路

1. 常见状态码

2. 缓存

3. cookie, session, token

4. 前端持久化的方式、区别

5. DNS是怎么解析的

6. cdn

7. 计算机网络的相关协议

8. http/https/http2.0

9. get post区别

10. ajax、 axios库

11. tcp三次握手，四次挥手流程

12. 跨域

13. 前端安全XSS、CSRF

14. websocket

15. Http请求中的keep-alive有了解吗

16. 网络分层

17. 即时通信，除了Ajax和websocket

18. 模块化，commonJS，es6，cmd，amd

### react

1. MVVM的理解
mvvm => modal+view+viewModel
modal:对应react 中组件的方法业务逻辑，redux+react-redux，
view:虚拟Dom转化的真实Dom.
viewmodel:jsx,vertal Dom的语法糖。

2. 如何实现一个自定义组件，不同组件之间如何通信的？
function 定义无状态组件
    > 组件不会被实力化，没有this对象，没有生命周期函数


extends React.Component
    > 

    父->子 props
    子->父 父传子function,子调用return value

    兄弟=> 共同父级状态 || redux

3. 生命周期

                        getDefaultProps
                        getInitialState
                        ComponentWillMount
                              render
                        ComponentDidMount
            <=           ShouldComponentUpdate         ComponentWillUnmount


4. 虚拟dom的原理

5. 单页应用，如何实现其路由功能---路由原理

6. redux

### 性能优化
1. 页面DOM节点太多，会出现什么问题？如何优化？

2. 如何做性能监测

3. SEO和语义化

### HTTP

1. 跨域
// 不同的域名、协议、端口会造成跨域
jsonp跨域
cors 后端控制跨域

2. HTTP 报文

3. 从输入 URL 到页面加载全过程

4. xss，csrf
xss又叫css,跨站脚本攻击分为：反射型、存储型、操作Dom
防范：将用户输入转码，服务端输出检查，HttpOnly

csrf:跨站请求伪造：截取信任用户向服务器发起请求
防范：添加验证码，使用token

### webpack

1. 打包原理
> 模块打包机制，识别模块依赖来打包项目代码。
主要功能：打包(将多文件打包成一个文件，减少服务力压力)；转化（将预编译语言转化成浏览器识别语言）；优化（性能优化，压缩）
> 把所有依赖打包成一个bundle.js文件，通过代码分割成单元片段并按需加载。

2. 打包插件
内置：ProvidePlugin ，引入$ jquery
打包：HtmlWebpackPlugin -> 重构入口文件，动态添加<Link><Script>
优化:UglifyJsPlugin(压缩代码)，CommonsChunkPlugin（合并公共组件为单独文件），MiniCssExtractPlugin

3. webpack热更新原理


4. 优化构建速度
webpack-bundle-analyzer，

### 算法

1. 排序算法

2. 字符串中找出最长最多重复的子串

3. 动态规划，参见背包问题

4. 层次遍历二叉树

5. 加油站问题(贪心算法)

6. 二分法

7. 单链表反转

8. 取1000个数字里面的质数

9. 找出数组中和为给定值的两个元素，如：[1, 2, 3, 4, 5]中找出和为6的两个元素。

10. 线性顺序存储结构和链式存储结构有什么区别？以及优缺点

