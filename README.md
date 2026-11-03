<p align="center">
  <img src="favicon.svg" width="72" height="72" alt="水印工坊 logo">
</p>

<h1 align="center">水印工坊 · 图片批量加水印</h1>

<p align="center">
  纯前端单文件图片水印工具 —— 拖入图片，30 秒批量加上专业水印。<br>
  零依赖 · 纯本地 · 可离线，图片不会被上传到任何服务器。
</p>

## ✨ 功能

- **文字水印**：支持多行文字、自定义颜色、透明度、旋转角度
- **图片 / Logo 水印**：上传本地 Logo，可调大小、透明度、旋转角度
- **平铺防盗**：密度、间距、角度可调，把水印均匀铺满整张图
- **九宫格定位**：点选左上 / 居中 / 右下… 等 9 个位置
- **批量处理**：多选或拖拽多张图片，一键导出 **ZIP**（可自定义文件名后缀）
- **导出设置**：格式（JPEG / WebP / 自动）、质量、缩放比例
- **完全本地**：所有渲染在浏览器 Canvas 中完成，无任何网络请求，断网也能用

## 🚀 使用

### 方式一：直接打开

双击 `index.html`，或拖进浏览器即可使用（推荐 Chrome / Edge）。

### 方式二：GitHub Pages

仓库开启 Pages（Source 选 `main` 分支根目录）后，访问：

```
https://GSHPChina.github.io/watermark-lab/
```

### 方式三：本地静态服务

```powershell
npx serve .
# 或
python -m http.server 8000
```

## 📁 项目结构

```
watermark-lab/
├── index.html      # 全部代码（HTML + CSS + JS 单文件，无构建步骤）
├── favicon.svg     # 站点图标
├── LICENSE         # MIT
└── README.md
```

## 🛠 技术

- 原生 HTML / CSS / JavaScript，**无任何框架和外部依赖**
- Canvas 2D 渲染水印，`toBlob` 导出
- 内联手写的 ZIP 打包器 `makeZip()`（Store 方式，零第三方库）
- 文件读取全部基于 `URL.createObjectURL`，用完即释放

## 📄 License

[MIT](LICENSE) © 2026 GSHPChina
