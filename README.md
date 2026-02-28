# 🏗️ 小塔阅读平台 - 完整版本

## 🎯 项目概述

小塔阅读是一个完整的在线阅读平台，包含6大核心功能模块，为用户提供专业的小说阅读体验。

## 📦 功能模块

### 1. 用户系统 👤
- 用户注册与登录
- 个人中心管理
- 阅读历史记录
- 书架收藏功能
- 密码安全加密

### 2. 完整阅读器 📖
- 流畅章节翻页
- 书签和笔记功能
- 阅读进度同步
- 夜间模式切换
- 字体大小调整

### 3. 书籍管理 📚
- 智能搜索功能
- 分类浏览系统
- 热门榜单推荐
- 收藏和书单管理
- 书籍详情展示

### 4. 智能推荐 🎯
- 个性化推荐算法
- 相似书籍推荐
- 阅读趋势分析
- 热门内容发现
- 实时更新推荐

### 5. 商业化功能 💰
- 付费章节系统
- 会员订阅服务
- 虚拟货币体系
- 支付集成支持
- 订单管理系统

### 6. 后台管理 🛠️
- 用户管理后台
- 书籍内容管理
- 数据统计分析
- 系统设置配置
- 操作日志审计

## 🚀 快速开始

### 环境要求
- Node.js 18+
- MongoDB 6.0+
- Redis 7.0+
- Docker 20.10+ (可选)

### 安装步骤

```bash
# 1. 克隆项目
git clone https://github.com/YOUR_USERNAME/xiaota.git
cd xiaota

# 2. 安装依赖
cd frontend && npm install
cd ../backend && npm install
cd ../admin && npm install

# 3. 配置环境变量
cp .env.example .env
# 编辑.env文件配置数据库等信息

# 4. 启动服务
# 启动后端
cd backend && npm start

# 启动前端 (新终端)
cd frontend && npm start

# 启动后台管理 (新终端)
cd admin && npm start
```

### Docker部署

```bash
# 使用Docker Compose一键部署
docker-compose up -d

# 访问应用
# 前端: http://localhost:3000
# 后端API: http://localhost:3001
# 后台管理: http://localhost:3002
```

## 📁 项目结构

```
xiaota/
├── frontend/          # 前端应用 (React + TypeScript)
├── backend/           # 后端API (Node.js + Express)
├── admin/             # 后台管理系统
├── docker-compose.yml # Docker容器编排
├── .env.example       # 环境变量示例
├── README.md          # 项目文档
└── docs/              # 详细文档
```

## 🔧 技术栈

### 前端技术
- **框架**: React 18 + TypeScript
- **样式**: Tailwind CSS + Styled Components
- **状态管理**: Redux Toolkit
- **路由**: React Router v6
- **构建工具**: Vite

### 后端技术
- **运行时**: Node.js 20
- **框架**: Express.js
- **数据库**: MongoDB + Mongoose
- **缓存**: Redis
- **认证**: JWT + Passport.js

### 部署技术
- **容器化**: Docker + Docker Compose
- **反向代理**: Nginx
- **CI/CD**: GitHub Actions
- **监控**: Prometheus + Grafana

## 📊 数据库设计

### 核心数据模型
- **用户表** (users): 用户信息和认证
- **书籍表** (books): 书籍信息和元数据
- **章节表** (chapters): 书籍章节内容
- **阅读记录** (reading_records): 用户阅读进度
- **订单表** (orders): 付费订单记录
- **推荐表** (recommendations): 个性化推荐数据

## 🔐 安全特性

- JWT令牌认证
- 密码加密存储 (bcrypt)
- CORS安全配置
- 请求速率限制
- SQL/NoSQL注入防护
- XSS攻击防护

## 📈 性能优化

- 数据库索引优化
- Redis缓存层
- CDN静态资源分发
- 图片懒加载
- 代码分割和懒加载
- 服务端渲染 (SSR)

## 🤝 贡献指南

1. Fork项目仓库
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 📞 支持

- **问题反馈**: [GitHub Issues](https://github.com/YOUR_USERNAME/xiaota/issues)
- **文档**: [项目文档](./docs/)
- **讨论**: [GitHub Discussions](https://github.com/YOUR_USERNAME/xiaota/discussions)

## 🎉 致谢

感谢所有为小塔阅读平台做出贡献的开发者和用户！

---

**最后更新**: 2026-02-28  
**版本**: v1.0.0  
**状态**: 🟢 生产就绪