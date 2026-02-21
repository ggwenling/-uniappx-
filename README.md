# 🌍 旅游小程序 Travel App

一个基于 uni-app x 和 uts,cool-unix 开发的精美旅游小程序，支持微信小程序平台。(不支持H5,需要下载微信开发工具)

## ✨ 功能特点

- 🏠 **首页**：瀑布流展示旅游景点，支持懒加载和无限滚动  /index
- 📍 **详情页**：景点详细信息展示，游玩推荐             /detail
- ❤️ **收藏页**：我的收藏列表，精美卡片设计            /like
- 👤 **个人中心**：用户信息管理，统计数据展示           /my
- 🗺️ **项目页**：地图展示，项目详情                    /project

## 🚀 性能优化

- ✅ 请求缓存机制（5分钟有效期）
- ✅ 防止重复请求（请求合并）
- ✅ 图片懒加载
- ✅ 瀑布流数据量限制（最多100条）
- ✅ 点击防抖（500ms）
- ✅ 页面卸载时自动清理资源

## 🛠️ 技术栈

- **框架**：uni-app x (uvue)
- **UI 组件库**：cool-ui
- **样式**：SCSS + Tailwind CSS
- **语言**：TypeScript + uts
- **构建工具**：Vite

## 📦 安装依赖

```bash
# 使用 pnpm（推荐）
pnpm install

# 或使用 npm
npm install

# 或使用 yarn
yarn install
```

## 🏃 运行项目

```bash
# 微信小程序开发
npm run dev:mp-weixin

# H5 开发
npm run dev:h5

# App 开发
npm run dev:app
```


## 📱 编译发布

```bash
# 编译微信小程序
npm run build:mp-weixin

# 编译 H5
npm run build:h5

# 编译 App
npm run build:app
```
##具体UI设计##
<img width="414" height="896" alt="06052cd6-45cc-4282-b74c-f3350a29ba51" src="https://github.com/user-attachments/assets/1df8b7c5-a003-4206-9eda-1ecd184d2f2c" />
<img width="414" height="896" alt="8a4f84e1-ba78-4377-9c84-17a1086b2dc6" src="https://github.com/user-attachments/assets/51869172-ee5d-4e51-a0a5-45ceddc78405" />
<img width="414" height="896" alt="7ead9113-1ead-4b8c-9ed7-f33de38c9dbb" src="https://github.com/user-attachments/assets/b6058d7d-811f-48a2-abf9-a51114b21a18" />
<img width="414" height="896" alt="e44e505b-3cfc-4e70-8b01-2879a9f29540" src="https://github.com/user-attachments/assets/d9b19823-9125-4a99-8973-9b9891442e74" />
<img width="414" height="896" alt="1e297a67-46aa-4f01-8629-cb619ad39c3e" src="https://github.com/user-attachments/assets/7628c598-29ed-4fc8-aaf6-713b4352741d" />


## 📂 项目结构

```
travel/
├── api/                  # API 接口封装
│   ├── api.ts           # 业务接口
│   └── request.ts       # 请求封装（带缓存）
├── pages/               # 页面文件
│   ├── index/          # 首页
│   ├── detail/         # 详情页
│   ├── like/           # 收藏页
│   ├── my/             # 个人中心
│   └── project/        # 项目页
├── static/             # 静态资源
├── uni_modules/        # uni-app 插件
├── App.uvue           # 应用入口
├── main.uts           # 主入口文件
├── pages.json         # 页面配置
└── manifest.json      # 应用配置
```

## 🎨 UI 设计亮点
- 依靠penci 设计的现代化UI
- 现代化渐变背景
- 流畅的动画过渡效果
- 精美的卡片设计
- 毛玻璃效果
- 响应式布局

## 📝 开发说明

### API 配置

在 `api/request.ts` 中修改 API 基础地址：

```typescript
const baseUrl = 'https://your-api-domain.com/api'
```

### 缓存配置

默认缓存时间为 5 分钟，可在 `api/request.ts` 中修改：

```typescript
const CACHE_TIME = 5 * 60 * 1000 // 5分钟
```


## 👨‍💻 作者

wenling

## 注意 ！！！##
本作者用的是别人的后端接口，其中搜索功能的接口已经失效，并且一些接口返回的图片部分是http格式，并非https，这使得一些图片无法在小程序上展示（尤其是真机测试时），往见谅,具体接口地址: https://s.apifox.cn/8776d148-3d28-42a1-bf4b-c2285ac6e644/api-266224381

