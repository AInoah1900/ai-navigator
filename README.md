# AI导航器 (AI-Navigator)

AI导航器是一个集合了各类AI工具和资源的导航网站，帮助用户快速找到并使用各种AI相关工具、服务和资讯。

## 项目概述

本项目是一个基于Next.js和React构建的现代化Web应用，提供了一个直观的界面来浏览和搜索各种AI工具和资源。项目采用了响应式设计，确保在不同设备上都能提供良好的用户体验。

## 功能特点

- **分类导航**：按照不同类别（如AI对话聊天、AI绘画、AI编程工具等）组织AI工具
- **搜索功能**：支持按名称搜索AI工具
- **响应式设计**：适配不同屏幕尺寸的设备
- **卡片式布局**：直观展示每个工具的名称、描述和图标
- **外部链接**：直接跳转到各AI工具的官方网站

## 技术栈

- **前端框架**：Next.js 15.1.7
- **UI库**：React 19.0.0
- **样式**：Tailwind CSS
- **UI组件**：Material UI (MUI)
- **语言**：TypeScript

## 项目结构

```
ai-navigator/
├── public/             # 静态资源文件夹
│   └── img/            # 工具图标图片
├── src/                # 源代码
│   └── app/            # Next.js应用目录
│       ├── components/ # 可复用组件
│       │   └── Navbar.tsx  # 导航栏组件
│       ├── card/       # 卡片详情页面
│       ├── globals.css # 全局样式
│       ├── layout.tsx  # 应用布局
│       └── page.tsx    # 主页面
├── data.json           # 工具数据
├── tailwind.config.ts  # Tailwind配置
├── tsconfig.json       # TypeScript配置
└── package.json        # 项目依赖
```

## 数据结构

项目使用 `data.json`文件存储所有AI工具的信息，按照不同类别组织。每个工具包含以下信息：

- **id**：唯一标识符
- **name**：工具名称
- **description**：工具描述
- **img**：工具图标（存储在public/img/目录）
- **link**：工具官方网站链接

## 安装与运行

### 前提条件

- Node.js 18.0.0或更高版本
- npm或yarn包管理器

### 安装步骤

1. 克隆仓库

```bash
git clone https://github.com/yourusername/ai-navigator.git
cd ai-navigator
```

2. 安装依赖

```bash
npm install
# 或
yarn install
```

3. 运行开发服务器

```bash
npm run dev
# 或
yarn dev
```

4. 打开浏览器访问 http://localhost:3000

### 构建生产版本

```bash
npm run build
npm run start
# 或
yarn build
yarn start
```

## 自定义与扩展

### 添加新工具

要添加新的AI工具，只需在 `data.json`文件中相应的类别下添加新的工具信息：

```json
{
  "id": "新ID",
  "name": "工具名称",
  "description": "工具描述",
  "img": "图标文件名.jpg",
  "link": "https://工具官网链接"
}
```

并将对应的图标文件放在 `public/img/`目录下。

### 添加新类别

要添加新的工具类别，在 `data.json`文件中添加新的类别对象：

```json
{
  "title": "新类别名称",
  "cards": [
    // 该类别下的工具列表
  ]
}
```

## 未来计划

- 添加用户评分和评论功能
- 实现工具使用统计和推荐系统
- 增加更多AI工具分类和资源
- 优化移动端体验
- 添加暗黑模式支持

## 贡献指南

欢迎对本项目做出贡献！请遵循以下步骤：

1. Fork本仓库
2. 创建您的特性分支 (`git checkout -b feature/amazing-feature`)
3. 提交您的更改 (`git commit -m 'Add some amazing feature'`)
4. 推送到分支 (`git push origin feature/amazing-feature`)
5. 开启一个Pull Request

## 许可证

本项目采用MIT许可证 - 详情请参阅LICENSE文件

## 联系方式

如有任何问题或建议，请通过以下方式联系我们：

- 项目GitHub: [https://github.com/AInoah1900/ai-navigator](https://github.com/yourusername/ai-navigator)
- 电子邮件: lxxc521@gmail.com

---

*本站所有内容均为AI生成*
