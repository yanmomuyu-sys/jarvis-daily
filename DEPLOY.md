# JARVIS AI 资讯日报 - GitHub Pages 部署指南

**状态**: 🟡 待手动操作

---

## 📋 待完成步骤

### 1. 创建 GitHub 仓库

**方式 A: GitHub Web 界面**（推荐）

1. 访问 https://github.com/new
2. Repository name: `jarvis-daily`
3. Description: "JARVIS AI 资讯日报 - 每日自动采集、摘要、推送 AI 领域最新动态"
4. Visibility: ✅ Public
5. 点击 "Create repository"

**方式 B: GitHub CLI**

```bash
gh repo create ujoker/jarvis-daily --public --description "JARVIS AI 资讯日报"
```

---

### 2. 推送代码

仓库创建后，执行：

```bash
cd /Users/ujoker/.openclaw/workspace/github-pages/jarvis-daily
git remote add origin https://github.com/ujoker/jarvis-daily.git
git branch -M main
git push -u origin main
```

---

### 3. 启用 GitHub Pages

1. 访问 https://github.com/ujoker/jarvis-daily/settings/pages
2. **Build and deployment**:
   - Source: Deploy from a branch
   - Branch: `main` → `/ (root)`
3. 点击 "Save"

---

### 4. 等待部署

- GitHub Actions 会自动触发
- 约 1-2 分钟完成部署
- 访问 https://ujoker.github.io/jarvis-daily/

---

## 🔍 验证部署

### 检查 Actions 状态

访问 https://github.com/ujoker/jarvis-daily/actions

- 应该看到 "Deploy to GitHub Pages" 工作流
- 状态应为 ✅ Success

### 访问网站

打开 https://ujoker.github.io/jarvis-daily/

应该看到：
- JARVIS AI 资讯日报首页
- Vol.001 日报内容
- 导航栏（首页/历史归档/关于）

---

## 🐛 故障排除

### 问题 1: 404 Not Found

**原因**: Pages 未启用或部署未完成

**解决**:
1. 检查 Pages 设置是否启用
2. 等待 Actions 完成
3. 清除浏览器缓存

### 问题 2: 样式丢失

**原因**: 主题未正确加载

**解决**:
1. 检查 `_config.yml` 中 theme 配置
2. 确认使用 minima 主题（GitHub Pages 默认支持）

### 问题 3: 推送失败

**原因**: 仓库不存在或权限问题

**解决**:
```bash
# 检查远程仓库
git remote -v

# 重新添加
git remote remove origin
git remote add origin https://github.com/ujoker/jarvis-daily.git

# 重新推送
git push -u origin main
```

---

## 📊 部署检查清单

- [ ] GitHub 仓库已创建
- [ ] 代码已推送
- [ ] Pages 已启用
- [ ] Actions 运行成功
- [ ] 网站可访问
- [ ] 首期日报显示正常
- [ ] 历史归档链接正常

---

## 🔗 相关链接

- **仓库**: https://github.com/ujoker/jarvis-daily
- **Pages**: https://ujoker.github.io/jarvis-daily/
- **Actions**: https://github.com/ujoker/jarvis-daily/actions
- **设置**: https://github.com/ujoker/jarvis-daily/settings/pages

---

**创建时间**: 2026-03-08 12:14  
**状态**: 🟡 待手动操作
