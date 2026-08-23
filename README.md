# PromptHub · AI生图提示词论坛

一个基于 GitHub Pages + GitHub JSON 数据存储的 AI 生图提示词分享论坛。

## 特性

- 提示词数据存储在 GitHub 仓库 `data/prompts.json`，多设备同步
- 支持 Pony Diffusion V6 XL、Animagine XL 3.1 等主流模型分类
- 9 大分类：写实、动漫、插画、赛博朋克、国风、3D渲染、概念艺术、人像
- 一键复制正向/负向提示词
- 搜索、筛选、排序、标签系统
- 点赞收藏（本地存储）
- 深浅色主题切换
- 管理员通过 GitHub Token 发布/编辑/删除提示词
- 响应式设计，移动端适配

## 部署到 GitHub Pages

1. 在 GitHub 创建仓库
2. 将本目录所有文件（包括 `data/` 文件夹）上传到仓库根目录
3. 仓库 Settings → Pages → Source 选择 `main` 分支 → Save
4. 等待 1-2 分钟，访问 `https://你的用户名.github.io/仓库名/`

## 管理员使用

1. 点击右上角齿轮图标进入管理后台
2. 输入 GitHub Personal Access Token（classic，勾选 repo 权限）
3. 验证成功后即可发布、编辑、删除提示词
4. 每次保存会自动提交到 GitHub 仓库，GitHub Pages 会自动重新部署

## Token 创建方法

1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token (classic)
3. Note 随便填，Expiration 选 No expiration
4. 勾选 `repo` 权限（完整仓库访问）
5. Generate token → 复制保存（只显示一次）

## 文件结构

```
/
├── index.html          # 主页面（所有代码）
├── data/
│   └── prompts.json    # 提示词数据（GitHub存储）
├── .nojekyll           # 禁用Jekyll处理
├── .gitignore
└── README.md
```

## 注意事项

- 普通访客无需登录即可浏览和复制提示词
- 只有配置了 Token 的管理员可以发布/编辑/删除
- 每次写入触发 GitHub Pages 重新部署，需等待 1-2 分钟
- 点赞和收藏数据存在浏览器本地，换设备不互通
