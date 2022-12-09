hugo基础操作

* `hugo new site SITE_NAME` 生成静态博客项目
* `hugo new post/new-content.md` 在 posts 下新建一篇文章
* `hugo server` 启动本地服务器，加上 `-D` 可以渲染 draft
* `hugo` 生成站点静态文件
* `hugo list drafts/expired/future` 列出特点的文件

克隆项目后，第一次拉取子模块：

```bash
cd wanfengedge.github.io
git submodule update --init --recursive
```

以后更新子模块

```bash
cd wanfengedge.github.io
git submodule update --remote
```
