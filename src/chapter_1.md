# Chapter 1

### book.toml

``` toml
[book]
title = "Example book"
authors = ["John Doe", "Jane Doe"]
description = "The example book covers examples."

[build]
build-dir = "book"
create-missing = true
preprocess = ["links", "index"]

[output.html]
theme = "my-theme"
curly-quotes = true
google-analytics = "123456"
additional-css = ["custom.css", "custom2.css"]
additional-js = ["custom.js"]

[output.html.playpen]
editor = "./path/to/editor"
editable = false

[output.html.search]
enable = true
searcher = "./path/to/searcher"
limit-results = 30
teaser-word-count = 30
use-boolean-and = true
boost-title = 2
boost-hierarchy = 1
boost-paragraph = 1
expand = true
heading-split-level = 3
copy-js = true
```

## 关于导入其他文件的两种方式

### playpen

我是这样写的`{{ #playpen ***}}` 

> *** == `./SUMMARY.md`

{{ #playpen ./SUMMARY.md}}

### include

我是这样写的`{{ #include ***}}`

> *** == `./SUMMARY.md`

{{ #include ./SUMMARY.md}}

下一节，是rust文件的导入，看看有什么不同