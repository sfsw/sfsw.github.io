[angularjs-web]: http://angularjs.org

<center>[![AngularJS](img/AngularJS.png)](https://angularjs.org/)</center>

#AngularJS 是什么？#
***
#### 概述 ####
> AngularJS 是一个 MV*（Model-View-Whatever，不管是 MVC 或者 MVVM，统归 MDV(model drive view)）JavaScript 框架，其是 Google 推出的SPA（single-page-application）应用框架。

#### 区别 ####
> **类库：**
> 一些在开发 Web 应用时非常有用的函数的集合。你的代码起主导作用，并且决定何时调用类库的方法。例如：jQuery 等。

> **框架：**
> Web 应用的特殊实现，你的代码只需要填充一些具体信息。框架起主导作用，并且决定何时调用你的代码。例如：Meteor, Backbone 等。

> **AngularJS：**
> AngularJS 提供的不是一部分解决方案，而是一个完整的解决方案，包括：数据绑定、指令、服务、路由、组件、依赖注入等，通过自定义的指令能让你以一种声明式的方法来扩展 HTML 功能。

# 特性 #
***
* **控制器(controller) - 应用的行为**
	* 控制器的主要工作内容是构造模型，并把模型和回调方法一起发送到视图。
* **模型(model) - 应用的数据**
	* 模型就是用来和模板结合生成视图的数据。和其他框架不一样的是，AngularJS 对模型本身没有任何限制和要求。
* **视图(view) - 用户能看到的**
	* 其他模板
		* 大部分模板都是一开始获取一个带有特殊标记的 HTML 形式字的字符串。但是这种特殊标记破坏了 HTML 的语法，以至于不能被 HTML 编辑器编辑。随后这个字符串会被送到模板引擎那里解析，并和数据合并。合并的结果是一个可以被浏览器解析的 HTML 字符串。这个字符串会被 .innerHTML 方法写到 DOM 中。使用 innerHTML 会造成浏览器的重新渲染。当模型改变时，这整个流程又要重复一遍。模板的生存周期就是 DOM 的更新周期。我想强调的是这些模板系统都是字符串。
	* AngularJS
		* AngularJS 和其它模板系统不同。它使用的是 DOM。模板仍然是用 HTML 字符串写的，并且它仍然是 HTML。浏览器将它解析成 DOM，然后这个 DOM 对象会传递给模板引擎，也就是 AngularJS 的编译器。编译器查看其中的指令，找到的指令后，会开始监视指令内容中相应的模型。这样做，就使得视图能“连续地”更新，不需要模板和数据的重新合并。你的模型也就成了你视图变化的唯一动因。
* **作用域(scope) - 视图和控制器的集合区（数据绑定）**
	* 作用域是控制器(controller)和视图(view)之间的纽带，我们只需要把模型(model)数据存放在作用域(scope)中就能起到双向绑定的作用。
	* ![示例图](img/diag1.jpg)
* **指令(directives) - 扩展HTML语法**
	* 指令能让你以一种声明式的方法来扩展 HTML 表示能力。
* **过滤器(filters) - 数据本地化**
	* 过滤器扮演着数据翻译的角色。它参照了UNIX过滤的规则，并且也实现了“|”（管道）语法。
* **注入器(injector) - 聚合你的应用**
	* inversion of control 控制反转（dependency injection 依赖注入，动态加载）

# 链接 #
***
* [AngularUI](http://angular-ui.github.io)
* [Web site][angularjs-web]
* [Tutorial](http://www.ngnice.com/docs/tutorial)
* [API Docs](http://www.ngnice.com/docs/api)
* [API Docs Backup](http://218.244.151.201:1339/docs/api)
* [Developer Guide](http://www.ngnice.com/docs/guide)
* [Contribution guidelines](http://www.ngnice.com/docs/misc/contribute)
* [Dashboard](http://www.ngnice.com/showcase)

```ver 1.0 by 苏佳晶 at 2014-8-11```