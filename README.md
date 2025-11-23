# Math 24 Game / 算24游戏

一个现代化的算24游戏，具有简洁的设计和流畅的动画效果。

A modern Math 24 game with minimalist design and smooth animations.

## 游戏介绍 / About

算24是一个经典的数学益智游戏。游戏会给出4个数字，你需要使用加减乘除运算符和括号，让这4个数字的运算结果等于24。

Math 24 is a classic mathematical puzzle game. You are given 4 numbers and need to use arithmetic operators (+, -, ×, ÷) and parentheses to make the result equal to 24.

## 功能特点 / Features

- 🎨 **简洁设计** - 现代化的极简主义卡片设计
- ✨ **流畅动画** - 平滑的悬停效果和过渡动画
- 🎆 **庆祝特效** - 答对时的烟花动画效果
- 💡 **智能提示** - 提供解题提示和鼓励信息
- 🎯 **即时反馈** - 实时验证答案正确性

## 如何游玩 / How to Play

1. 点击"新游戏"开始一局新游戏
2. 点击数字卡片和运算符来构建表达式
3. 使用括号来控制运算顺序
4. 点击"确认"提交你的答案
5. 如果需要帮助，点击"查看提示"

## 本地开发 / Local Development

直接在浏览器中打开 `index.html` 即可运行游戏。

Simply open `index.html` in your browser to run the game.

```bash
# 使用本地服务器运行（推荐）
# Run with a local server (recommended)
python3 -m http.server 8000
# 然后访问 http://localhost:8000
```

## 在线访问 / Live Demo

游戏已部署到 GitHub Pages，可以在线访问：

The game is deployed on GitHub Pages:

🎮 [在线游玩 / Play Online](https://statcafehk.github.io/math24game/)

## 技术栈 / Tech Stack

- HTML5
- CSS3 (原生CSS动画)
- JavaScript (原生JS)
- 纯前端实现，无需后端服务器

## 💡 技术实现亮点 / Technical Highlights

### 纯前端架构 / Pure Frontend Architecture

这个项目采用了**完全前端实现**的设计理念，无需任何后端服务器或 API：

- ✅ **零服务器成本** - 完全静态托管，可免费部署到 GitHub Pages
- ✅ **即时响应** - 所有计算在本地完成，无网络延迟
- ✅ **离线可用** - 下载后可完全离线使用
- ✅ **隐私保护** - 所有数据都在用户浏览器中，不上传任何信息

### 智能解题算法 / Solution Algorithm

游戏使用**暴力搜索算法**在前端实时计算所有可能的解法：

```javascript
// 核心算法流程
1. 生成所有数字排列 (4! = 24 种)
2. 尝试所有运算符组合 (4³ = 64 种)
3. 尝试不同括号模式 (9 种)
4. 总计算量: 24 × 64 × 9 = 13,824 种可能性
```

**性能表现**：
- 每次发牌时，浏览器在**几毫秒内**完成所有计算
- 即使在移动设备上也能流畅运行
- 算法复杂度：O(n! × m³ × p)，其中 n=4, m=4, p=9

### 为什么选择前端实现？ / Why Frontend-Only?

**优势**：
1. **部署简单** - 只需一个 HTML 文件，拖到任何静态服务器即可
2. **成本为零** - 无需购买服务器、数据库或 API 服务
3. **扩展性强** - 可以轻松添加更多功能而不增加基础设施成本
4. **学习友好** - 代码完全开源，适合学习前端算法和动画

**权衡**：
- 无法收集全局统计数据（可通过 localStorage 实现本地统计）
- 算法代码对用户可见（但这也是开源的优势）
- 无法实现多人对战（可通过 WebRTC 等技术扩展）

### 代码亮点 / Code Highlights

1. **SVG 卡片渲染** - 使用原生 SVG 绘制扑克牌，无需图片资源
2. **CSS 动画** - 纯 CSS 实现烟花效果，性能优异
3. **函数式编程** - 使用递归算法生成排列组合
4. **本地存储** - 使用 localStorage 持久化游戏统计

## 项目结构 / Project Structure

```
math24game/
├── index.html              # 主页面（包含所有代码）
├── README.md               # 项目说明
├── .gitignore              # Git忽略文件
└── docs/                   # 文档目录
    ├── README.md                        # 文档索引
    ├── game_features_walkthrough.md     # 功能演练
    ├── deployment_walkthrough.md        # 部署指南
    ├── github_deployment_guide.md       # GitHub 部署
    ├── github_pages_setup.md            # Pages 设置
    ├── implementation_plan.md           # 实施计划
    └── media/                           # 媒体文件
        ├── encouraging_popup_*.png      # 截图
        ├── fireworks_final_*.png        # 截图
        └── fireworks_demo_*.webp        # 演示视频
```

## 更新日志 / Changelog

### v1.0.0 (2025-11-22)
- ✨ 初始版本发布
- 🎨 极简主义卡片设计
- 🎆 烟花庆祝动画
- 💡 智能提示系统
- 📱 响应式设计

## 许可证 / License

MIT License

---

Made with ❤️ | 用心制作
