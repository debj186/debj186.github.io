# 代码折叠

<details>
    <summary><span style='background-image:linear-gradient(to right, orange, purple);
                    color:transparent;
                    -webkit-background-clip:text;'>启动类</span></summary>
    <pre><code>public static void main(String[] args) {
  SpringApplication.run(ServerApplication.class, args);
}</code></pre>
</details>

# 版本差异

```diff
- var a = 'hello world'
- console.log(a）
+ console.log('hello')
+ console.log('hello world')
```

# Typora 主题

[Typora 主题-中文站](https://theme.typoraio.cn/) 中选择 Drake

```css
/**
 * drake-dark.css 添加内容
 *
 * 自定义拓展：导航栏右悬浮、标题颜色、标题序号
 */

.md-toc {
    float: right;
    position: fixed;
    right: 45px;
    top: 17.6%;
    width: 316px;
    max-height: 52.8%;
    overflow-y: auto;
    margin-top: 0px;
    padding-bottom: 0px;
    z-index: 1000;
}

#write {
    counter-reset: h1;
	cursor: text;
	transform: inherit;
}

h1 {
    counter-reset: h2;
	/* color: #f9963b; */
    font-size: 2rem;
    text-align: left;
    margin-top: 36px;

    /* 渐变色：暗红-橘黄 */
    display: block;
    width: fit-content !important;
	margin-bottom: 0px;
    color:transparent;
    -webkit-background-clip:text;
    background-image: linear-gradient(to right, #da3369, #db720b);
}

h1:nth-of-type(1){
    margin-top: 0;
}

h2 {
    counter-reset: h3;
	/* color: #46ACC8; */
    font-size: 1.4rem;
    
    /* 渐变色：绿-蓝 */
    display: block;
    width: fit-content !important;
    padding: 0px;
    margin: 28px 0px 8px 0px;
    color:transparent;
    -webkit-background-clip:text;
    background-image: linear-gradient(to right, #cca202, #15834c, #14884e);
}

h2 .md-plain {
    padding-bottom: 0px;
    border-bottom: 0;
    line-height: 0px;
}

h3 {
    counter-reset: h4;
    color: #31a5c0;
    font-size: 1.2rem;
}

h4 {
    font-size: 1.2rem;
}

h5 {
    font-size: 1.2rem;
}

h6 {
    font-size: 1.2rem;
}

#write h1:before {
    counter-increment: h1;
    content: counter(h1) ". "
}

#write h2:before {
    counter-increment: h2;
    content: counter(h1) "." counter(h2) " "
}

#write h3:before, h3.md-focus.md-heading:before {
    counter-increment: h3;
    content: counter(h1) "." counter(h2) "." counter(h3) " "
}

#write h4:before, h4.md-focus.md-heading:before {
    counter-increment: h4;
    content: counter(h1) "." counter(h2) "." counter(h3) "." counter(h4) " "
}

#write h5:before, h5.md-focus.md-heading:before {
    counter-increment: h5;
    content: counter(h1) "." counter(h2) "." counter(h3) "." counter(h4) "." counter(h5) " "
}

#write h6:before, h6.md-focus.md-heading:before {
    counter-increment: h6;
    content: counter(h1) "." counter(h2) "." counter(h3) "." counter(h4) "." counter(h5) "." counter(h6) " "
}

#write > h3.md-focus:before,
#write > h4.md-focus:before,
#write > h5.md-focus:before,
#write > h6.md-focus:before,
h3.md-focus:before,
h4.md-focus:before,
h5.md-focus:before,
h6.md-focus:before {
    color: inherit;
    border: inherit;
    border-radius: inherit;
    position: inherit;
    left: inherit;
    float: inherit;
    top: inherit;
    font-size: inherit;
    padding-left: inherit;
    padding-right: inherit;
    vertical-align: inherit;
    font-weight: inherit;
    line-height: inherit;
    visibility: inherit;
}
```
