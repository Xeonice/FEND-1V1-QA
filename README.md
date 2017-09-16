# FEND 前端24期日常1V1 Q&A集
<br>

   * [FEND 前端24期日常1V1 Q&amp;A集](#fend-前端24期日常1v1-qa集)
      * [8.21 - 8.27](#821---827)
         * [Q：是否应该用其他方式巩固自己CSS方面学习成果？](#q是否应该用其他方式巩固自己css方面学习成果)
         * [Q：Grunt是否对今后项目有影响？压缩图片的基本原理是怎样的？](#qgrunt是否对今后项目有影响压缩图片的基本原理是怎样的)
         * [Q：DIV什么时候会被默认为inline的？](#qdiv什么时候会被默认为inline的)
         * [Q：有没有直接拖动组件进行布局的网页布局？](#q有没有直接拖动组件进行布局的网页布局)
         * [Q：CSS集成库推荐？](#qcss集成库推荐)
      * [8.28-9.4](#828-94)
         * [Q: Bootstrap文档应该在哪里查阅？](#q-bootstrap文档应该在哪里查阅)
         * [Q: 是否应该现在接触 Vue.js ?](#q-是否应该现在接触-vuejs-)
         * [Q：命名函数表达式的函数名为什么只在新定义的函数作用域内有效？而函数声明时的函数名在整个函数的作用域范围内均有效？](#q命名函数表达式的函数名为什么只在新定义的函数作用域内有效而函数声明时的函数名在整个函数的作用域范围内均有效)
         * [Q：“AlbERt EINstEiN” 除最后一个单词外的其余单词按照首字母大写，其余字母小写的格式输出，这样操作可行吗？](#qalbert-einstein-除最后一个单词外的其余单词按照首字母大写其余字母小写的格式输出这样操作可行吗)
      * [9.4 - 9.11](#94---911)
         * [Q: display: inline 能与 <code>float</code> 属性实现相近的效果，那么这两个 <code>CSS</code> 属性有什么区别呢？](#q-display-inline-能与-float-属性实现相近的效果那么这两个-css-属性有什么区别呢)
         * [Q: 盒子模型和容器的概念有些混淆](#q-盒子模型和容器的概念有些混淆)
         * [Q: CSS中直接在 img 标签中给图片统一设置高度为什么没有反应？](#q-css中直接在-img-标签中给图片统一设置高度为什么没有反应)
         * [Q: P3 Making Peach Ice Cream Tests](#q-p3-making-peach-ice-cream-tests)
         
<br>

## 8.21 - 8.27

### Q：是否应该用其他方式巩固自己CSS方面学习成果？
**A:** 可考虑参照现有的，自己喜欢的网站进行临摹，运用CSS，HTML实现与目标网站相同的样式
### Q：Grunt是否对今后项目有影响？压缩图片的基本原理是怎样的？
**A:** `Grunt`就和`Photoshop`里面的插件一样，它能够帮我们自动完成一些反复重复的任务
ps插件里，我们经常会用动自动切图，自动导出切片这样的工具。`Grunt`里面，就可以使用自动编译LESS、压缩CSS、JS这样的工具。

Grunt压缩图片的基本原理与大部分图片压缩工具的原理基本相同，具体可参见：[Web性能优化：图片优化](http://web.jobbole.com/81766/)。
### Q：DIV什么时候会被默认为inline的？
**A:** `Div`作为块级元素，其默认值为`block`，如果想将其转为`inline`元素，需要主动设置`display: inline`。

关于块级，行内元素的详细信息可见：[block，inline和inline-block概念和区别](http://www.cnblogs.com/KeithWang/p/3139517.html)
### Q：有没有直接拖动组件进行布局的网页布局？
**A:** 详情参照[Layoutit](http://layoutit.justjavac.com)，一套简单的拖动布局系统。
### Q：CSS集成库推荐？
**A:** [Bootstrap](http://www.bootcss.com)，一套极为成熟的CSS框架系统。
<br>
## 8.28-9.4
### Q: Bootstrap文档应该在哪里查阅？
**A:** 详情可见[Bootstrap中文网](http://v3.bootcss.com/)。
### Q: 是否应该现在接触 `Vue.js` ?
**A:** `Vue.js` 的官方介绍中明确指出：
> 官方指南假设你已有 HTML、CSS 和 JavaScript 中级前端知识。
> 如果你刚开始学习前端开发，将框架作为你的第一步可能不是最好的主意——掌握好基础知识再来！
> 之前有其他框架的使用经验对于学习 Vue.js 是有帮助的，但这不是必需的。

因此，在学习 `Vue.js` 前建议先完成前端入门学位的学习。
### Q：命名函数表达式的函数名为什么只在新定义的函数作用域内有效？而函数声明时的函数名在整个函数的作用域范围内均有效？

> 例如：

> ```
> var func1 = function func2(){
>     console.log("hello");
> }
> ```
> `func2`函数名只能在`func2`函数内部调用，而在外面调用不了。

**A:** `ECMAScript` 规范中规定：
> 
```
var bar = function foo() {};
```
该函数表达式是一个有效的命名函数表达式，但是有一点要记住，这个名字只在新定义的函数作用域内有效，因为规范规定了标示符不能在外围的作用域内有效。

### Q：“AlbERt EINstEiN” 除最后一个单词外的其余单词按照首字母大写，其余字母小写的格式输出，这样操作可行吗？

> 例如： 
> 
```
function nameCharger(oldName) {
    var finalName = "";
    var names = [];
    // 以空格分割字符串
    names = oldName.split(" ");
    console.log(name.length);
    //将单词首字母大写，其他字母小写
    for(var i = 0; i < names.length; i++){
        names[i] = names[i].toLowerCase();
        console.log(names[i]);
        names[i][0] = names[i][0].toUpperCase();
        console.log(names[i]);
        finalName += names[i];
        finalName += " ";
    }
    names[names.length-1] = names[names.length-1].toUpperCase;
    finalName += names[names.length - 1];
```

**A:** `ECMAScript` 中规定：
> `ECMAScript` 中的字符串是不可变的，也就是说，字符串一旦创建，它们的值就不能改变。要改变某个变量保存的字符串，首先要销毁原来的字符串，然后再用另一个包含新值的字符串填充该变量。

也就是说，当我们在进行 `names[i] = names[i].toLowerCase();` 操作时，原先的字符串在运算中就被销毁了，因此，该操作是不可行的。
<br>
## 9.4 - 9.11
### Q: `display: inline` 能与 `float` 属性实现相近的效果，那么这两个 `CSS` 属性有什么区别呢？
**A:** 详情可参看[详解CSS中的display属性（行内元素和块级元素）](https://segmentfault.com/a/1190000000654770)，[inline-block和float的共性和区别](http://www.cnblogs.com/scot/p/5501669.html)这两篇文章。
### Q: 盒子模型和容器的概念有些混淆
**A:** 可参见[详解CSS盒模型
](http://luopq.com/2015/10/26/CSS-Box-Model/)。
### Q: CSS中直接在 `img` 标签中给图片统一设置高度为什么没有反应？
**A:** 可以尝试把 `img` 放在 `div` 容器里，然后在 `div` 容器中加入 `width` 和 `height`。
### Q: P3 Making Peach Ice Cream Tests
<br>
#### Q: 用 `<li>` 标签里设置 `float： left` 或者 `<ul>` 中设置 `display: inline` 都可以达到目的，但是插件提示错误？
**A:** 在 `<li>` 中设置 `display: inline` 即可。
#### Q: The recipe is centered inside the paper background处，设置 `margin: 0 auto` 却无法通过？
**A:** 参见 [制作桃子口味的冰淇淋中的“margin:0 auto”问题](https://discussions.youdaxue.com/t/margin-0-auto/42698/6) 中 **Zhilian** 的回答
#### Q: Homemade 右侧的图片没有与标题同行？
**A:** `recipe` 里面设置了 `width` ， 还有一个 `padding` ， 去掉即可。
<br>
## 9.11 - 9.18
### Q: 使用 `Font Awesome` CDN 时如何更改图标样式？例如大小／位置？
**A:** CDN上Download下来的样式是无法被直接更改的，因此，我们可以通过为目标元素添加父容器 `div` ，在父容器 `div` 上进行样式的更改来完成相应目标。
PS：IconFont相关可以参见[Iconfont-阿里巴巴矢量图标库](http://www.iconfont.cn/)，相较于 `Font Awesome` 加载速度更快，更加本土化。
### Q: 必须挂 VPN 才能安装 grunt 插件吗？
**A:** `grunt` 插件利用 `npm` 包管理工具进行管理，因此，可以考虑更换 `npm` 的下载源为[淘宝NPM镜像](http://npm.taobao.org)。
### Q: P3 部分该如何使用栅格布局？
**A:** 可以参见[栅格系统](http://v3.bootcss.com/css/#grid)，并参照 `BootStrap` 源代码进行布局。
### Q: 使用 BootStrap 框架必须要在每一个项目中都下载一个 BootStrap 项目文件夹吗？
**A:** CSS文件可通过CDN引用的方式进行加载。具体使用方法可参见[使用 BootCDN 提供的免费 CDN 加速服务（同时支持 http 和 https 协议）](http://v3.bootcss.com/getting-started)。
<br>
## 9.18 - 9.25


