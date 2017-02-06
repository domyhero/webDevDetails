## 前言

* 请记住，这篇文档并不是实际搭建一个网页项目，而是告诉我们怎么从零开始搭建一个工程化的网页项目，所以主要要告诉的就是我们在这一过程中思路是怎么样的！通过这篇文档，能让大家了解相关框架、工具的使用原理以及以及如何构建自动化项目。**_诚然，前端技术日新月异，各种框架满天飞，所以自己在某些方面也感觉到不足，所以还请看到该文档的前辈能够不吝不吝赐教，请移步_**[这里](https://github.com/woai30231/webDevDetails/issues)

* 假定现实情况：假设有个网页需求，有一个主页index.html，有三个子页contact.html、introduct.html、product.html，这三个子页分别从index.html连接过来，又可以从三个子页返回index.html。我们采用spa的方式构建单页面app，采用grunt管理前台代码程序，采用bower管理各种第三方依赖库。最终项目在[这里]()

* **注意：本文档已经默认你有js、css、html基础，并且知道了解angularjs框架！**

### 开始着手完成项目

* 我们每做一个事情，都会在心里有个默认次序，先做什么，再做什么，最后做什么，依次类推！我们搭建这个项目也是一样，我们需要先确定每一步该做什么，以此来理清思绪！

#### 第一步：确定项目结构

* 如何熟悉angular搭建项目的目录结构的话，我们就采用下面的目录结构来组织我们的app

> app
>> contact

>>> contact.css

>>> contact.js

>>> contact.controller.js

>>> contact.html

>> introduct

>>> introduct.css

>>> introduct.js

>>> introduct.controller.js

>>> introduct.html

>> product

>>> product.js

>>> product.css

>>> product.controller.js

>>> product.html

>> index.html

>> app.js

采用这样的结构方便我们把每一个路由当作一个模块，从而方便管理每个页面下的css、js等！