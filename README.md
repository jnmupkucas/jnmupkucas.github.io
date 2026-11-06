# Jianan Mu — Academic Homepage

静态学术主页，包含最新的 23 篇代表论文、分类筛选、中英文简介切换、校徽和 CV。
无需 Node.js、依赖安装、编译或后端，可直接用于 GitHub Pages。

## 发布到 GitHub Pages

1. 创建公开仓库，推荐名称：`你的GitHub用户名.github.io`（将用户名替换为实际账号）。
2. 解压本代码包，把文件夹内的全部文件与 `assets` 目录上传至仓库根目录。
   确保 `index.html` 直接位于仓库根目录，不要多套一层文件夹；不要只上传 ZIP 文件。
3. 打开仓库 **Settings → Pages**。
4. 在 **Build and deployment** 中选择 **Source: Deploy from a branch**。
5. 选择 **Branch: main**、**Folder: / (root)**，点击 **Save**。
6. 等待部署完成，在 Pages 设置页点击访问链接。

仓库名为 `你的GitHub用户名.github.io` 时，访问地址是 `https://你的GitHub用户名.github.io/`。
普通仓库也可以使用，地址是 `https://你的GitHub用户名.github.io/仓库名/`；页面使用相对资源路径，兼容两种方式。

## 文件说明

- `index.html`：主页全部 HTML、CSS 和 JavaScript；论文数据在 `const papers` 数组中。
- `assets/cas.jpg`：中国科学院院徽。
- `assets/pku.png`：北京大学校徽。
- `Jianan_Mu_CV.pdf`：用户提供的原始简历，供下载。
- `.nojekyll`：让 GitHub Pages 直接提供静态文件（网页上传若遗漏此空文件，不影响当前页面资源）。

## 后续修改

修改简介、经历或服务：编辑 `index.html` 中对应文字。
新增论文：编辑 `const papers` 数组。每条论文的字段依次是：
`年份、会议/期刊、分类、标题、作者、作者角色、奖项、论文链接`。
分类值：`verification`（Verification & Reliability）或 `ai`（AI for Chip Design）。
当前论文按验证与可靠在前、AI 与加速器设计在后的顺序展示。
Faver 的期刊发表年份未在所提供简历中注明，因此暂未展示年份。

替换简历时保留文件名 `Jianan_Mu_CV.pdf`，即可继续使用现有下载按钮。
注意：附带 PDF 是原始上传版本，其职称仍为 Assistant Researcher；主页按要求写为 Assistant Professor。

校徽来源：中国科学院官网、北京大学视觉形象识别系统下载专区。

## 本地预览

直接双击 `index.html` 即可预览，也可以在该目录运行 `python -m http.server 8000` 后访问 `http://localhost:8000/`。

## GitHub 官方文档

- https://docs.github.com/en/pages/quickstart
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
