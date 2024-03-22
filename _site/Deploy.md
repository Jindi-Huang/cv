# 如何部署基于Jekklly，af-folio主题的个人主页
## 1. 更改信息
基本信息位于`_config.yml`文件中，包括网站标题、作者等信息，根据自己的需求进行修改。

主题配色位于`_sass/_variables.scss`文件中，主题位于`_sass/_theme.scss`文件中，可根据自己的需求进行修改。

所有页面均位于`_pages`文件夹中，其中大部分多余页面已经设置为不显示，即`nav : false`。

所有图片位于`assets/images`文件夹中，包括论文预览图，位于`assets/image/publication_preview`文件夹中。

所有pdf文件位于`assets/pdf`文件夹中，包括论文pdf，cv等。

Json格式的cv位于`assets/json`文件夹中，文件名为`resume.json`。

所有文章的bib文件位于`_bibliography`文件夹中，文件名为`papers.bib`，采用bibtex格式。

较多功能已经被移除，如需添加可参考原主题 [af-folio](https://github.com/alshedivat/al-folio)，并直接询问l

## 2. 上传代码
将代码上传到GitHub仓库中，仓库名为`username.github.io`，其中`username`为你的GitHub用户名。

## 3. 部署网站
1. 进入GitHub仓库，点击`Settings`，找到`General`选项，将`Default branch` rename为`source`。
2. 进入`Github Pages`选项，设置`Source`为`Github Actions`.
3. 更新任意文件并push，触发Github Actions，等待部署完成。