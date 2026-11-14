# 我的学术主页

[Jinnuo Li (李金诺)](https://jinnuoli.github.io/)

主页使用 [al-folio v1.2](https://github.com/alshedivat/al-folio/releases/tag/v1.2) 的主题样式、导航和配色脚本，使用 Jekyll 和 Jekyll-Scholar 生成页面。

- 修改个人简介、教育经历、学术服务和安全报告时，编辑 `_pages/about.html`。
- 修改论文时，编辑 `_bibliography/papers.bib`。标有 `selected = {true}` 的论文也会显示在首页，完整论文页会按年份自动分组。
- 本地预览可运行 `bundle install` 和 `bundle exec jekyll serve`。

GitHub Pages 从 `main` 分支的根目录直接提供预生成页面。修改内容后，在仓库根目录构建并更新两个 HTML 文件，再一并提交：

```sh
bundle exec jekyll build
ruby -rfileutils -e "FileUtils.cp('_site/index.html', 'index.html'); FileUtils.cp('_site/publications/index.html', 'publications/index.html')"
```
