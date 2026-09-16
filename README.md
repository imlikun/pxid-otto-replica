# PXID × Otto Hofstetter 版式复刻（中文）

基于 https://www.otto-hofstetter.swiss/ 的布局、动画、交互（Webflow 导出），
将内容、图片、文案替换为 **PXID 电动出行**（pxid.com）语境的复刻站点。

## 保留（原站）
- 版式 / 动画 / 交互 / 结构
- 品牌色（Otto 蓝 `#00A1E5`）
- 阿尔卑斯山景等氛围背景
- LinkedIn 动态墙等第三方组件

## 替换（PXID）
- 全部产品、工艺、认证、博客、客户故事、hero 文案
- 图片素材来自 pxid.com（产品 / 工艺 / 认证图标）
- 品牌词 Otto Hofstetter → PXID，文案中文化并去 AI 腔

## 本地预览
```bash
# 任意目录起静态服务（示例 8890）
python -m http.server 8890 --directory . --bind 127.0.0.1
# 打开 http://127.0.0.1:8890/index.html
```

## 结构
- `index.html` — 首页
- `pages/` — 31 个内页（文件名与站内链接一致）
- `assets/` — 图片 / CSS / JS / 字体
- `media/` — 视频 / 动效素材

## 校验
打包脚本 `package_delivery.py` 已做全量内链硬校验（2282 条相对链接 0 缺失）。
