# Chapter 1

### book.toml

示例

``` toml
{{ #include ../book.toml}}
```

## 关于导入其他文件的两种方式

### playpen

我是这样写的`{{ #playpen ***}}` 

> `***` == `./SUMMARY.md`

{{ #playpen ./SUMMARY.md}}

### include

我是这样写的`{{ #include ***}}`

> `***` == `./SUMMARY.md`

{{ #include ./SUMMARY.md}}

下一节，是rust文件的导入，看看有什么不同