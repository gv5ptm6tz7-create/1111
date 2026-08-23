# PromptHub · AI生图提示词论坛

一个纯前端、离线可用的 AI 生图提示词分享社区，支持完整的后台可视化管理。

## ✨ 功能特性

### 前台功能
- 🏠 **首页**：数据统计、热门分类、热门提示词、最新发布、活跃创作者
- 🔍 **发现页**：分类筛选、模型筛选、标签筛选、关键词搜索、4种排序、网格/列表双视图、分页
- 📄 **详情页**：正向/负向Prompt展示、一键复制、生成参数、相关推荐、点赞/收藏/评论
- ✏️ **发布页**：分组表单、标签输入、参数配置，支持编辑已有提示词
- 👤 **个人中心**：我的发布、我的收藏、我的点赞、浏览历史
- 🌓 **深色/浅色主题**一键切换
- ⌨️ **快捷键**：`Ctrl+K` 聚焦搜索，`Esc` 关闭弹窗

### 后台管理（点击导航栏 ⚙️ 图标进入）
- 📊 **仪表盘**：数据概览、热门TOP5、分类/模型分布图表
- 📝 **提示词管理**：查看/编辑/删除所有提示词
- 🏷️ **分类管理**：可视化新增/编辑/删除分类，自定义图标
- 🤖 **模型管理**：新增/编辑/删除模型，设置HOT标签，自定义主题颜色
- 💬 **评论管理**：查看/删除所有评论
- 👥 **用户管理**：用户列表与统计
- 💾 **数据备份**：导出JSON备份、导入恢复、重置默认数据
- ⚙️ **系统设置**：网站名称/描述、每页数量、默认主题、功能开关

## 🚀 部署到 GitHub Pages

### 方法一：直接上传（最简单）

1. 登录 GitHub，点击右上角 **+** → **New repository**
2. 仓库名随意填（例如 `ai-prompt-forum`），选择 **Public**，点击 **Create repository**
3. 在仓库页面点击 **uploading an existing file**
4. 把本压缩包解压后的**所有文件**（`index.html`、`README.md`、`.nojekyll` 等）拖进去
5. 点击 **Commit changes**
6. 进入仓库 **Settings** → 左侧 **Pages**
7. **Source** 选择 `Deploy from a branch`，**Branch** 选择 `main` / `(root)`，点击 **Save**
8. 等待 1-2 分钟，页面上方会显示你的网站地址，例如：
   `https://你的用户名.github.io/ai-prompt-forum/`

### 方法二：使用 GitHub Desktop

1. 安装 [GitHub Desktop](https://desktop.github.com/)
2. 登录后点击 **File** → **Add local repository**，选择解压后的文件夹
3. 点击 **Publish repository** 发布到 GitHub
4. 按方法一的第 6-8 步开启 Pages

## 📁 项目结构

```
ai-prompt-forum/
├── index.html      # 主程序（单文件应用，包含所有HTML/CSS/JS）
├── README.md       # 说明文档
├── .nojekyll       # 告诉 GitHub Pages 跳过 Jekyll 处理
└── .gitignore      # Git 忽略规则
```

## 💾 数据说明

- 所有数据（提示词、分类、模型、评论、设置、点赞收藏、浏览历史）存储在浏览器的 **localStorage** 中
- 数据仅保存在当前浏览器，换浏览器或清除缓存会丢失
- 建议定期在后台 **数据备份** 页面导出 JSON 文件做备份
- 导出的 JSON 文件可在任意设备的后台导入恢复

## 🎨 内置模型

- Pony Diffusion V6 XL 🔥
- Animagine XL 3.1 🔥
- Midjourney
- Stable Diffusion
- DALL-E 3
- Nijijourney

可在后台 **模型管理** 中自由增删改。

## 📝 内置分类

写实、动漫、插画、赛博朋克、国风、3D渲染、概念艺术、人像

可在后台 **分类管理** 中自由增删改。

## 🔧 技术栈

- 纯 HTML + CSS + JavaScript（单文件，无任何外部依赖）
- 无需后端服务器，无需数据库
- 支持所有现代浏览器（Chrome、Edge、Firefox、Safari）

## 📄 License

MIT
