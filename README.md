# FCAR 论文项目页

本仓库为论文 **FCAR: Force-Conditioned Action Residual Policies for Contact-Rich Manipulation** 的项目网站，风格参考 [Nerfies](https://nerfies.github.io)。

## 本地预览

在项目根目录下启动任意静态服务器，例如：

```bash
# Python 3
python -m http.server 8000

# 或 Node.js
npx serve .
```

浏览器打开 `http://localhost:8000` 即可查看。

## 添加图片

将论文中的图导出为 PNG 后放入 `static/images/`，并确保文件名与页面引用一致：

| 文件名 | 对应论文内容 |
|--------|--------------|
| `teaser.png` | 图1（Teaser） |
| `architecture.png` | figs (2).pdf（方法框架图） |
| `exp_setup.png` | figure/exp_prepare.pdf（实验设置） |

也可在 `index.html` 中修改 `src` 路径以使用你自己的命名。若某张图不存在，页面会显示占位说明而不会报错。

## 效果展示视频

**视频放在：`static/videos/`**

- **主视频**：将论文/项目的效果展示视频命名为 **`teaser.mp4`** 并放入 `static/videos/`，页面上的「Video」区块会自动引用并播放。
- 支持 **MP4**（推荐，兼容性好）；若使用其他格式，可在 `index.html` 里为 `<video>` 增加对应 `<source>` 标签。
- 若使用 **YouTube 或 B 站**：在 `index.html` 的 Video 区块中按注释说明，把 iframe 打开并填入视频 ID 即可（可同时保留或去掉本地 `<video>`）。

## 部署到 GitHub Pages

1. 在 GitHub 新建仓库（如 `fcar-manipulation.github.io` 或 `username.github.io/repo`）。
2. 将本目录内容推送到该仓库。
3. 仓库设置中开启 GitHub Pages，源选择 main 分支根目录（或 docs 目录，若你把网站放在 docs 下）。

## 修改链接

在 `index.html` 中可修改：

- **Paper**：PDF 链接（如会议/arXiv 正式版）
- **arXiv**：arXiv 摘要页
- **Project**：项目页链接

本项目代码不开源，页面仅保留 Paper / arXiv / Project 链接。作者信息目前为 “Anonymous Author(s)”，投稿后可改为真实作者与单位。

## 许可

页面结构参考 Nerfies 项目页，内容与图片版权归论文作者所有。
