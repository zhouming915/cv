# 周明 · UI设计师 个人作品集网站

这是一个使用GSAP ScrollTrigger创建的现代化个人作品集网站。

## 功能特点

- 🎨 现代化设计风格，深色主题
- 📱 完全响应式布局
- ✨ 平滑的滚动触发动画（GSAP ScrollTrigger）
- 🎯 多个动画区域：卡片、时间轴、项目展示、技能展示
- 📊 动态统计数字
- 🔄 3D旋转盒子固定动画
- 📝 优雅的文字揭示效果

## 网站结构

```
zhouming-portfolio/
├── index.html          # 主页面
├── images/            # 项目截图文件夹
│   ├── project-1.png
│   ├── project-2.png
│   └── ...
└── README.md         # 本文件
```

## 主要区域

1. **Hero区域** - 个人介绍和座右铭
2. **设计理念** - 三个核心设计理念卡片
3. **职业历程** - 时间轴展示工作经历
4. **精选项目** - 10个项目展示（支持hover效果）
5. **设计技能** - 软件logo展示 + 统计数字
6. **设计过程** - 固定动画区域
7. **愿景展示** - 文字揭示效果
8. **联系信息** - 联系方式

## 技术栈

- HTML5
- CSS3 (Grid, Flexbox, 自定义属性)
- JavaScript (原生)
- GSAP 3.12.5
  - GSAP Core
  - ScrollTrigger 插件

## 本地预览

直接用浏览器打开 `index.html` 文件即可预览。

或者使用本地服务器：

```bash
# Python 3
python -m http.server 8000

# 然后访问 http://localhost:8000
```

## 部署到GitHub Pages

### 方法一：从main分支部署

1. 在GitHub上创建新仓库（例如：`zhouming-portfolio`）
2. 将整个 `zhouming-portfolio` 文件夹推送到仓库：

```bash
cd zhouming-portfolio
git init
git add .
git commit -m "Initial commit: 个人作品集网站"
git remote add origin https://github.com/你的用户名/zhouming-portfolio.git
git push -u origin main
```

3. 在GitHub仓库设置中启用GitHub Pages：
   - 进入仓库 → Settings → Pages
   - Source 选择 "Deploy from a branch"
   - Branch 选择 "main" 和 "/ (root)"
   - 点击 Save

4. 等待1-2分钟，访问 `https://你的用户名.github.io/zhouming-portfolio/`

### 方法二：使用gh-pages分支

```bash
# 安装GitHub CLI（如果还没有）
# 然后直接部署
git push origin main
```

## 自定义修改

### 修改个人内容

编辑 `index.html` 中的以下内容：

- **Hero区域** (第720-736行): 修改姓名、职位、简介
- **时间轴** (第757-801行): 修改工作经历
- **项目展示** (第803-887行): 修改项目信息和图片
- **联系信息** (第976-993行): 修改邮箱、电话、地址

### 修改颜色主题

编辑 `index.html` 中的CSS变量（在第9-700行的`<style>`标签内）：

- 主色调：`<style>` 标签中查找 `#667eea` 和 `#764ba2`（渐变色）
- 背景色：查找 `#0a0a0a` 和 `#141322`
- 文字色：查找 `#ffffff`、`#b0b0b0` 等

## 性能优化建议

- ✅ 已使用CDN加载GSAP（减少加载时间）
- ✅ 图片已优化（保持原始格式）
- 建议：部署前压缩图片（使用 tinypng.com）
- 建议：启用GitHub Pages的HTTPS

## 浏览器兼容性

- ✅ Chrome (推荐)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ⚠️ IE11 不支持（需要polyfill）

## 许可证

MIT License - 可自由使用和修改

## 联系方式

- 邮箱：155281067@qq.com
- 电话：189-5301-6373
- 常驻：北京

---

**Dream by Design** - 用设计将梦想变成现实
