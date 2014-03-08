Prototype
=========

#### 一个面向对象的JavaScript框架 ####

Prototype 是一个简化开发动态web应用的JavaScript框架。它提供了一个非常熟悉的`class-style`面向对象的风格的框架,扩展了Ajax支持，高级编程结构，易用的DOM操作。

### 支持平台 ###

当前支持如下平台:

* 微软Windows系统IE6或者更高版本，
* 火狐浏览器Mozilla Firefox 1.5 and higher
* 苹果浏览器Apple Safari 2.0.4 and higher
* 欧朋浏览器Opera 9.25 and higher
* 谷歌浏览器Chrome 1.0 and higher

使用 Prototype
---------------

要在你应用中使用Prototype,可从Prototype(<http://prototypejs.org/download>) 站点下载最新版本，或者复制该资源库目录下`dist/prototype.js`的源文件到你需要的位置。在你HTML引用他。
像这样:

    <script type="text/javascript" src="/path/to/prototype.js"></script>

### 使用资源文件来构建Prototype ###

`prototype.js` 是由该目录`src/`下许多个资源文件合并生产的一个复合文件。为了构建它，
你需要:

* a copy of the Prototype source tree, either from a distribution tarball or
  from the Git repository (see below)
* Ruby 1.8.2 or higher (<http://www.ruby-lang.org/>)
* Rake--Ruby Make (<http://rake.rubyforge.org/>)
* RDoc, if your Ruby distribution does not include it

定位到prototype根目录,

* `rake dist` will preprocess the Prototype source using Sprockets and 
  generate the composite `dist/prototype.js`.
* `rake package` will create a distribution tarball in the 
  `pkg/` directory.

贡献Prototype
-------------------------

用git获取 Prototype资源库，步骤如下

    $ git clone git://github.com/sstephenson/prototype.git
    $ cd prototype
    $ git submodule init
    $ git submodule update vendor/sprockets vendor/pdoc vendor/unittest_js

了解如何贡献: <http://prototypejs.org/contribute>.

文档
-------------

请查阅在线PrototypeAPI: <http://api.prototypejs.org>.
