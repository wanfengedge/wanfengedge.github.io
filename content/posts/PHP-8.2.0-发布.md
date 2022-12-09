---
title: "PHP 8.2.0 发布"
subtitle: ""
date: 2022-12-09T12:33:01+08:00
lastmod: 2022-12-09T12:33:01+08:00
draft: false
author: ""
authorLink: ""
description: ""
license: ""
images: []

tags: ["php"]
categories: ["php"]

featuredImage: ""
featuredImagePreview: ""

hiddenFromHomePage: false
hiddenFromSearch: false
twemoji: false
lightgallery: true
ruby: true
fraction: true
fontawesome: true
linkToMarkdown: true
rssFullText: false

toc:
  enable: true
  auto: true
code:
  copy: true
  maxShownLines: 50
math:
  enable: false
  # ...
mapbox:
  # ...
share:
  enable: true
  # ...
comment:
  enable: true
  # ...
library:
  css:
    # someCSS = "some.css"
    # located in "assets/"
    # Or
    # someCSS = "https://cdn.example.com/some.css"
  js:
    # someJS = "some.js"
    # located in "assets/"
    # Or
    # someJS = "https://cdn.example.com/some.js"
seo:
  images: []
  # ...
---
PHP 开发团队[宣布](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2Farchive%2F2022.php%232022-12-08-1)了 PHP 8.2.0 的立即可用，这是 PHP 语言的最新次要版本。

<!--more-->

PHP 8.2 带来了许多改进和新功能，例如：

* [只读类](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2Fmanual%2Fen%2Flanguage.oop5.basic.php%23language.oop5.basic.class.readonly) (Readonly classes)

将一个类标记为只读会给每个声明的属性添加只读修饰符，并阻止动态属性的创建。此外，不可能通过使用 AllowDynamicProperties 属性来增加对它们的支持。试图这样做将触发一个编译时错误。

```
<?php
#[AllowDynamicProperties]
readonly class Foo {
}

// Fatal error: Cannot apply #[AllowDynamicProperties] to readonly class Foo
?>
```

当且仅当子类也是一个只读类的时候，一个只读类可以被扩展。

* [析取范式 (DNF) 类型](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2Fmanual%2Fen%2Fmigration82.new-features.php%23migration82.new-features.core.type-system)
* 新的独立类型：[null、false](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwiki.php.net%2Frfc%2Fnull-false-standalone-types) 和 [true](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwiki.php.net%2Frfc%2Ftrue-type)
* [新的 “Random” 扩展](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2Fmanual%2Fen%2Fbook.random.php)
* [traits](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2Fmanual%2Fen%2Fmigration82.new-features.php%23migration82.new-features.core.constant-in-traits) [中的常量](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2Fmanual%2Fen%2Fmigration82.new-features.php%23migration82.new-features.core.constant-in-traits)
* [弃用动态属性](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2Fmanual%2Fen%2Fmigration82.deprecated.php%23migration82.deprecated.core.dynamic-properties)。动态属性的创建已被弃用，除非该类通过使用 `#[\AllowDynamicProperties]` 属性选择加入。 [stdClass](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2Fmanual%2Fen%2Fclass.stdclass.php) 允许动态属性。__get()/__set() magic methods 的使用不受此更改的影响。动态属性弃用警告可以通过以下方式解决：
  * 声明属性（首选）。
  * 将 `#[\AllowDynamicProperties]` 属性添加到类（这也适用于所有子类）。
  * 如果需要将额外的数据与一个不属于自己的对象相关联，则使用 [WeakMap 。](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2Fmanual%2Fen%2Fclass.weakmap.php)

更多详情可查看 [ChangeLog](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwww.php.net%2FChangeLog-8.php%238.2.0)。

下载地址：[https://windows.php.net/download/](https://www.oschina.net/action/GoToLink?url=https%3A%2F%2Fwindows.php.net%2Fdownload%2F)
