# Xinhao Tong 的个人主页

使用 Jekyll 和 AcademicPages 构建，发布地址为 <https://xinhaot.github.io/>。

- 首页内容、项目简介和联系方式：`_pages/about.md`
- 姓名、头像、侧栏邮箱和网站配置：`_config.yml`
- 顶部导航：`_data/navigation.yml`
- 联系邮箱：<xinhaot@zju.edu.cn>
- 项目网址：<https://xinhaot.github.io/ARAP-Deformation-of-Gaussian-Radiance-Fields/>

模板自带的示例论文、博客、项目、教学、演讲、简历、演示页面、评论及相关附件已清理。保留了主题、个人头像，以及可复用的数据生成工具；生成工具中的示例数据和 Notebook 输出已清空。

## 上传到 GitHub

本地仓库的 `origin` 已指向 `https://github.com/XinhaoT/XinhaoT.github.io.git`，当前分支为 `master`。在当前目录运行：

```bash
git status
git add -A
git commit -m "Clean template examples and add project and contact information"
git push origin master
```

`git add -A` 会同时提交新增、修改和删除，因此 GitHub 上的示例文件也会被删除。若 HTTPS 推送要求认证，请使用 GitHub Personal Access Token 或已配置的凭据管理器。

## 开启 GitHub Pages

1. 打开 [GitHub 仓库](https://github.com/XinhaoT/XinhaoT.github.io)。使用 GitHub Free 时，需要将仓库设为 Public。
2. 进入 **Settings → Pages**。
3. 在 **Build and deployment → Source** 中选择 **Deploy from a branch**。
4. 选择 **master** 分支和 **/ (root)** 目录，点击 **Save**。
5. 在 **Actions** 中查看 Pages 构建和部署结果。部署成功后，访问 <https://xinhaot.github.io/>，或在 Pages 设置页点击 **Visit site**。

发布更新可能需要最多约 10 分钟。之后只需继续向 `master` 推送修改，GitHub Pages 就会自动更新网站。无需自己购买服务器或保持本机运行。

该仓库使用 Jekyll：不要添加 `.nojekyll`，也不要将发布目录设为 `/docs`。`_config.yml` 已配置：

```yaml
url: https://xinhaot.github.io
baseurl: ""
repository: XinhaoT/XinhaoT.github.io
```

如果访问返回 404，先确认 Pages 的分支和目录设置，再查看 Actions 中是否构建失败；还未完成的部署不会显示新内容。

参考：[GitHub Pages 发布源设置](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)、[创建和访问 GitHub Pages 网站](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)。

## 可选：本地预览

安装 Ruby 和 Bundler 后运行：

```bash
bundle install
bundle exec jekyll serve --config _config.yml,_config.dev.yml
```

浏览器打开 <http://localhost:4000>。修改 `_config.yml` 后需要重启预览服务。本地预览不是 GitHub Pages 发布的前提。

## 主题来源

基于 [AcademicPages](https://github.com/academicpages/academicpages.github.io) 和 [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes)，遵循仓库中的 MIT [LICENSE](LICENSE)。
