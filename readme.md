## mdbook 好的 例子 (60%,亦可用)

类(gitbooks)文档，专服务于Rust语言的md文档

> mdbook本身，还有很多小 bug，所以使用过程 **不要过于纠结**

### 请安装mdbook

```
cargo install mdbook
```

> 覆盖旧版本，需要`--force`

更多[安装信息](https://github.com/chinanf-boy/mdBook-zh#%E5%AE%89%E8%A3%85)

### 看看

- clone

```
git clone https://github.com/chinanf-boy/mdbook-nice-example.git
```

- `cd` *, look html

```
mdbook serve --open
```

### book.toml + src/SUMMARY.md

[book.toml]是配置，[src/SUMMARY.md](./src/SUMMARY.md)就是书的骨架

> 其实，本库就是一个模范示例, 直接clone魔改就好。当然你还能用`mdbook init --theme`拿到原始示例。

### 模范?,有啥

- [x] **1.** 加了个编辑按钮

可通过，在`index.hbs`[修改成自己的源项目地址](./src/theme/index.hbs#L163)

<details>
<summary>例子</br></summary>

> `src/theme/index.hbs`

``` hbs
document.getElementById("edit-button").addEventListener("click", function(){
    var editWindow = window.open("https://github.com/chinanf-boy/mdbook-nice-example/edit/master/src/{{ path }}");
});
```

`chinanf-boy/mdbook-nice-example` 改成你的 存储库，

</details>
</br>

- [ ] **2.** `git_repository_url` 不成功

``` toml
git_repository_url = "https://github.com/chinanf-boy/mdbook-nice-example"
git_repository_icon = "fa-github"
```

且，hbs模版是[有添加的](./src/theme/index.hbs#L128)，我想这就是bug吧

- [x] anything，其他杂七杂八的都在[book.toml]

> **NOTE >** Issue me , If you have question with this repo.
> But, about the bug of mdbook, please Link [that Source Issue Page](https://github.com/rust-lang-nursery/mdBook)

### 相关

[book.toml]: book.toml

- [mdbook 中文文档](https://github.com/chinanf-boy/mdbook-zh)