## mdbook 好的 例子 (未完成❎)

### 请安装mdbook

```
cargo install mdbook
```

> 覆盖旧版本，需要`--force`

更多[安装信息](https://github.com/chinanf-boy/mdBook-zh#%E5%AE%89%E8%A3%85)

### 看看

```
git clone https://github.com/chinanf-boy/mdbook-nice-example.git
```

```
mdbook serve --open
```

### 加了,有啥

- **1.** 加了个编辑按钮

可通过，在`index.hbs`[修改成自己的源项目地址](./src/theme/index.hbs#L158)

<details>
<summary>例子</summary>

> `src/theme/index.hbs`

``` hbs
document.getElementById("edit-button").addEventListener("click", function(){
    var editWindow = window.open("https://github.com/chinanf-boy/mdbook-nice-example/edit/master/src/{{ path }}");
});
```

`chinanf-boy/mdbook-nice-example` 改成你的 存储库，

</details>




### 相关

- [mdbook 文档](https://github.com/chinanf-boy/mdbook-zh)