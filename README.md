# MyBlog

基于 [Hexo](https://hexo.io/) 构建的个人博客站点。

## 技术栈

- **框架**: Hexo 8.x
- **主题**: Landscape
- **渲染器**: Markdown (marked)、EJS、Stylus
- **部署**: Git 部署器

## 快速开始

### 环境要求

- [Node.js](https://nodejs.org/) >= 14
- [Git](https://git-scm.com/)

### 安装

```bash
git clone <你的仓库地址>
cd Myblog
npm install
```

### 本地开发

启动本地服务器，默认地址为 `http://localhost:4000`：

```bash
npm run server
# 或
npx hexo server
```

### 创建新文章

```bash
npx hexo new "我的新文章"
```

文章文件将生成在 `source/_posts/` 目录下，使用 Markdown 编写。

### 生成静态文件

```bash
npm run build
# 或
npx hexo generate
```

生成的静态文件位于 `public/` 目录。

### 清理缓存

```bash
npm run clean
```

### 部署

```bash
npm run deploy
```

## 项目结构

```
Myblog/
├── _config.landscape.yml  # 主题配置文件
├── source/
│   └── _posts/            # 博客文章（Markdown）
├── scaffolds/             # 文章模板
├── themes/                # 主题文件
├── public/                # 生成的静态文件（构建产物）
├── node_modules/          # 依赖包
└── package.json           # 项目配置
```

## 常用命令

| 命令 | 说明 |
|------|------|
| `npm run server` | 启动本地开发服务器 |
| `npm run build` | 生成静态文件 |
| `npm run clean` | 清除缓存和生成的文件 |
| `npm run deploy` | 部署到远程站点 |
| `npx hexo new "标题"` | 创建新文章 |
| `npx hexo new page "页面"` | 创建新页面 |

## 相关链接

- [Hexo 官方文档](https://hexo.io/zh-cn/docs/)
- [Hexo GitHub](https://github.com/hexojs/hexo)
- [Landscape 主题](https://github.com/hexojs/hexo-theme-landscape)
