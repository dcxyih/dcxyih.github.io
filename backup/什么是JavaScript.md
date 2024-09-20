# 什么是JavaScript

JavaScript 是一门用来与网页交互的脚本语言

1995 年，JavaScript 问世。主要用途是代替 Perl 等服务器端语言处理输入验证。

## 简短的历史
1995 年，网景公司一位名叫 Brendan Eich 的工程师，开始为即将发布的 Netscape Navigator 2 开发一个叫 Mocha（后来改名为 LiveScript）的脚本语言。当时的计划是在客户端和服务器端都使用它，它在服务器端叫 LiveWire。

为了赶上发布时间，网景与 Sun 公司结为开发联盟，共同完成 LiveScript 的开发。就在 Netscape 
Navigator 2 正式发布前，网景把 LiveScript 改名为 JavaScript，以便搭上媒体当时热烈炒作 Java 的顺风车。

1996 年 8 月，微软重磅进入 Web 浏览器领域，这是网景永远的痛，但它代表 JavaScript 作为一门语言向前迈进了一大步。微软的 JavaScript 实现意味着出现了两个版本的 JavaScript：Netscape Navigator 中的 JavaScript，以及 IE 中的 JScript。

1997 年，JavaScript 1.1 作为提案被提交给欧洲计算机制造商协会（Ecma）。第 39 技术委员会（TC39）承担了“标准化一门通用、跨平台、厂商中立的脚本语言的语法和语义”的任务（参见 TC39-ECMAScript）。TC39 委员会由来自网景、Sun、微软、Borland、Nombas 和其他对这门脚本语言有兴趣的公司的工程师组成。他们花了数月时间打造出 ECMA-262，也就是 ECMAScript（发音为“ek-ma-script”）这个新的脚本语言标准。

1998 年，国际标准化组织（ISO）和国际电工委员会（IEC）也将 ECMAScript 采纳为标准（ISO/ 
IEC-16262）。自此以后，各家浏览器均以 ECMAScript 作为自己 JavaScript 实现的依据，虽然具体实现各有不同。


## JavaScript实现
完整的 JavaScript 实现包含以下几个部分：
- 核心（ECMAScript）

Web 浏览器只是 ECMAScript 实现可能存在的一种宿主环境（host environment）。宿主环境提供
ECMAScript 的基准实现和与环境自身交互必需的扩展。扩展（比如 DOM）使用 ECMAScript 核心类型
和语法，提供特定于环境的额外功能。其他宿主环境还有服务器端 JavaScript 平台 Node.js 和即将被淘汰的 Adobe Flash。

ECMA-262 到底定义了什么？
（语法
类型
语句
关键字
保留字
操作符
全局对象）

ECMAScript 只是对实现这个规范描述的所有方面的一门语言的称呼。

ECMA-262 第 6 版，**俗称 ES6**、ES2015 或 ES Harmony（和谐版），于 2015 年 6 月发布。这一版包含了大概这个规范有史以来最重要的一批增强特性。ES6 正式支持了类、模块、迭代器、生成器、箭头函数、期约、反射、代理和众多新的数据类型。

要成为 ECMAScript 实现，必须满足下列条件：  

1.支持 ECMA-262 中描述的所有“类型、值、对象、属性、函数，以及程序语法与语义”；  
2.支持 Unicode 字符标准。  
3.增加 ECMA-262 中未提及的“额外的类型、值、对象、属性和函数”。ECMA-262 所说的这些额
外内容主要指规范中未给出的新对象或对象的新属性。  
4.支持 ECMA-262 中没有定义的“程序和正则表达式语法”（意思是允许修改和扩展内置的正则表
达式特性）。


- 文档对象模型（DOM）

文档对象模型（DOM，Document Object Model）是一个应用编程接口（API），用于在 HTML 中使
用扩展的 XML。DOM 将整个页面抽象为一组分层节点。HTML 或 XML 页面的每个组成部分都是一种
节点，包含不同的数据。

DOM 通过创建表示文档的树，让开发者可以随心所欲地控制网页的内容和结构。使用 DOM API，可以轻松地删除、添加、替换、修改节点。

为了保持 Web 跨平台的本性，万维网联盟（W3C，World Wide Web Consortium）开始了制定 DOM 标准的进程。

- 浏览器对象模型（BOM）
  
浏览器对象模型（BOM） API

BOM 主要针对浏览器窗口和子窗口（frame），不过人们通常会把任何特定于浏览器的扩展都归在 BOM 的范畴内。