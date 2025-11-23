# 🚀 启用 GitHub Pages - 图文教程

## ✅ 当前进度

- ✅ Git 仓库已初始化
- ✅ 代码已推送到 GitHub
- ✅ 仓库地址：https://github.com/statcafehk/math24game

## 📋 接下来：启用 GitHub Pages

### 步骤 1：进入仓库设置

1. 打开你的仓库页面：https://github.com/statcafehk/math24game
2. 点击页面顶部的 **Settings**（设置）标签

### 步骤 2：找到 Pages 设置

1. 在左侧菜单中，向下滚动找到 **Pages** 选项
2. 点击 **Pages**

### 步骤 3：配置部署源

在 **Build and deployment** 部分：

1. **Source** (源)：选择 **Deploy from a branch**
2. **Branch** (分支)：
   - 第一个下拉菜单：选择 **main**
   - 第二个下拉菜单：选择 **/ (root)**
3. 点击 **Save** 按钮

### 步骤 4：等待部署完成

1. 保存后，页面会自动刷新
2. 等待 1-2 分钟，GitHub 会自动部署你的网站
3. 刷新页面，顶部会出现一个绿色的提示框，显示：

```
Your site is live at https://statcafehk.github.io/math24game/
```

## 🎮 访问你的游戏

部署完成后，你的 Math 24 游戏将在以下地址可用：

### 🌐 在线地址
**https://statcafehk.github.io/math24game/**

你可以：
- ✅ 分享这个链接给朋友
- ✅ 在任何设备上访问
- ✅ 无需安装任何软件

## 🔄 如何更新已部署的网站

当你修改代码后，只需要推送到 GitHub，网站会自动更新：

```bash
cd /Users/ajzhang/MyCode/math24game

# 修改文件后...
git add .
git commit -m "描述你的修改"
git push

# 等待 1-2 分钟，网站会自动更新
```

## ✅ 验证清单

部署完成后，访问网站并测试：

- [ ] 页面能正常加载
- [ ] 点击"新游戏"能生成新的数字
- [ ] 点击卡片和运算符能构建表达式
- [ ] 点击"确认"能提交答案
- [ ] 答对时能看到烟花动画
- [ ] 点击"查看提示"能看到鼓励信息

---

**完成后，请告诉我部署是否成功！** 🎉
