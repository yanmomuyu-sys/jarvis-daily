# JARVIS AI 资讯日报

> 每日清晨，为您精选 AI 领域最新动态

[![Deploy to GitHub Pages](https://github.com/ujoker/jarvis-daily/actions/workflows/deploy.yml/badge.svg)](https://github.com/ujoker/jarvis-daily/actions/workflows/deploy.yml)
[![Last Updated](https://img.shields.io/github/last-commit/ujoker/jarvis-daily/main)](https://github.com/ujoker/jarvis-daily/commits/main)

---

## 📰 关于

**JARVIS AI 资讯日报** 是一个自动化的 AI 资讯聚合系统，每日自动采集、摘要、推送 AI 领域最新动态。

**数据来源**:
- 行业新闻（Hacker News, TechCrunch）
- 热门开源项目（GitHub Trending）
- 前沿学术论文（arXiv）
- 社区讨论（Reddit, 知乎）
- 社交媒体（Twitter KOL）

**输出渠道**:
- 📱 Telegram 推送（简洁版）
- 🌐 GitHub Pages（完整版）

---

## 🚀 快速开始

### 订阅 Telegram

关注 [@ujoker](https://t.me/ujoker) 接收每日推送。

### 浏览网页版

访问 https://ujoker.github.io/jarvis-daily/ 查看完整日报。

### RSS 订阅

```
https://ujoker.github.io/jarvis-daily/feed.xml
```

---

## 📊 今日概览

查看 [今日日报](index.md)

---

## 📁 历史归档

- [2026-03-08 - Vol.001](_posts/2026-03-08-jarvis-daily.md)

[查看更多](/archive/)

---

## 🛠️ 技术栈

- **数据采集**: web_search, web_fetch
- **AI 摘要**: Qwen3.5-Plus (Bailian)
- **发布推送**: Telegram Bot API
- **网页展示**: GitHub Pages + Jekyll
- **自动化**: OpenClaw Cron

---

## 📅 更新频率

**每日 07:00** (Asia/Shanghai) 自动更新

---

## 📝 使用示例

### 手动触发

```bash
cd ~/.openclaw/workspace
./skills/public/daily-news-curator/scripts/daily-news-curator.sh all
```

### 查看日志

```bash
tail -20 reports/daily/daily-news-execution.log
```

---

## 🎯 功能特性

- ✅ 自动数据采集（20+ 数据源）
- ✅ AI 智能摘要（Qwen3.5-Plus）
- ✅ Telegram 推送（简洁版）
- ✅ GitHub Pages 展示（完整版）
- ✅ 历史归档（完整）
- ✅ RSS 订阅（支持）
- ✅ 错误重试（3 次）
- ✅ 质量检查（自动）
- ✅ 降级模式（容错）

---

## 📊 统计

| 指标 | 值 |
|------|-----|
| 数据源 | 20+ 个 |
| 每日采集 | 50+ 条 |
| 精选内容 | 10 条左右 |
| 阅读时间 | 5-10 分钟 |
| 运行时间 | ~13 秒 |

---

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

## 📄 许可证

MIT License

---

## 🔗 链接

- **GitHub**: https://github.com/ujoker/jarvis-daily
- **Telegram**: https://t.me/ujoker
- **OpenClaw**: https://openclaw.ai

---

**创建时间**: 2026-03-08  
**维护人**: JARVIS  
**状态**: 🟡 测试中
