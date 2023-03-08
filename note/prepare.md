# 准备

## 0. 感想

本来想认真地写一写，也许能有人能从中获取到编程的知识。但是，现在发现，我貌似没有输出的能力，写的乱七八糟的。

那只能说，我就写着玩吧。很尴尬~ 😂

## 1. 安装 Rust

偷懒不想介绍怎么安装 Rust。请参看别人的教程，顺便也推荐一下别人的书，😂。

[Rust语言圣经 #安装 Rust](https://course.rs/first-try/installation.html)

## 2. 开发工具

强烈推荐 [Visual Studio Code](https://code.visualstudio.com/)。

同时需要安装 rust-analyzer 插件。

---

> 多摸索，多思考，就会知道如何使用。基本的一些操作，网上真的教程很多的。

## 3. 梦开始的地方

在命令行界面，选择好代码放置的目录。（需要会基本的 shell 操作）
执行如下命令:
```sh
cargo new hello
```
将会得到一个初始化的项目。能够看到会生成一个名为 hello 的目录。

主要有 2 个文件: Cargo.toml 和 src 下的 main.rs
```
hello
    ├── Cargo.toml
    └── src
        └── main.rs
```
目前能说的，代码可以在文件 main.rs 里面编写。
> 貌似还不理解什么是 *代码*。😂

## 4. 第一次运行执行

进入 hello 目录，执行命令:
```sh
cargo run
```
可以看到界面会输出
```
Hello, world!
```
表明已经运行成功，并且看到代码输出的结果了。这个 "Hello, world!"，就是那个 main.rs 里面的代码做的事情了。

我们当前的任务就是在这个 main.rs 里面写一些代码，让计算机做我们让它做的事情。比如：计算一下 1+1 等于几 😂

---

一旦 run 了之后，会生成一个 target 目录和 Cargo.lock 文件。谁知道是干什么的呢 😠

## 5. 查看 main.rs 文件
用 vscode 打开 hello 目录。选择 main.rs 文件查看内容。
```rs
fn main() {
    println!("Hello, world!");
}
```

如果有行号
```rs
1 fn main() {
2     println!("Hello, world!");
3 }
```

后面第一次编写代码的地方就是第 2 行，所在的位置了，其他的东西暂时还是先不要关心了。
只要知道在第 2 行那个 println!... 的位置写代码，也就是告诉计算机做啥子，就行了。