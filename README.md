# Yubo Wang — Academic Homepage

个人学术主页：https://yubowang-zxx.github.io/

极简静态网页，采用 HTML + CSS；无需安装依赖或构建。GitHub Pages 从 `main` 分支的根目录发布，提交修改后会自动更新网站。

## 文件结构

- `index.html`：个人简介和 Selected Research Projects，已添加注释标记编辑区域。
- `assets/style.css`：字体、间距、页面宽度和手机端布局。
- `assets/Yubo_Wang_CV.pdf`：网站上的简历下载文件。
- `assets/` 中的图片：项目和论文插图。
- `ASSET-SOURCES.json`：图片来源记录。
- `.nojekyll`：让 GitHub Pages 直接提供静态文件。

## 常见修改

**修改文字或链接**：编辑 `index.html`，找到对应 section 或 article，修改后提交。文字中的 `&` 写成 `&amp;`，不要删掉成对的 HTML 标签。

**更新简历**：用新 PDF 替换 `assets/Yubo_Wang_CV.pdf`，保持文件名相同即可。

**增加项目**：复制一整段 `<article class="research-item"> ... </article>`，更新标题、日期、链接、摘要和图片。给 `id` 一个新的唯一值。无图片时使用 `research-item text-only` 并去掉 figure。

**更换照片**：替换 `assets/yubo-wang.jpg`。页面使用 CSS 调整显示范围，点击可查看原图。

**更新日期**：页面底部的 Last updated 为手动文本，修改内容时一并更新。

## 本地查看

下载整个仓库后，用浏览器打开 `index.html`，或在仓库目录执行 `python3 -m http.server 8000`，访问 http://localhost:8000。请保留 assets 文件夹与 index.html 的相对位置。

## 发布设置

仓库 Settings → Pages：Deploy from a branch，选择 `main` / `(root)`。无需单独的自定义构建工作流。修改后等待 GitHub Pages 的部署完成即可。

## 设计与图片来源

排版参考 [Jon Barron 的学术主页模板](https://github.com/jonbarron/jonbarron.github.io)，以及用户指定的 [Gaoyue Zhou](https://gaoyuezhou.github.io/) 和 [Rex Liu](https://rexliu9.github.io/) 主页。没有复制他人的个人内容或头像。

项目图片来自本人的课程报告、展示文件以及合作论文的 companion repository。图表保持原样，来源详见 ASSET-SOURCES.json。模板作者允许个人主页使用；论文、照片和项目材料保留各自的权利与归属。
