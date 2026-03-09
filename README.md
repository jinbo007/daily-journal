# 每日 AI 时间线网站

## 🌐 访问地址

**GitHub Pages**：https://jinbo007.github.io/daily-journal/

---

## ✅ 已完成

### 1. 网站功能
- ✅ AI 哲学展示（信息 → 决策 → 执行）
- ✅ 每日时间线（3月5-9日记录）
- ✅ 点击查看详情页面
- ✅ 统计面板（记录天数、主题、洞察）
- ✅ 响应式设计

### 2. 已部署内容
- **3月5日**：投资规划 · 资产配置优化
- **3月6日**：腾讯财报深度分析 · 阿里对比 · OpenClaw场景
- **3月9日**：AI 世界构建 · 技能部署 · 个人主页升级

### 3. 自动化脚本
- ✅ `update-timeline.sh` - 每日自动更新时间线
- ✅ 从 `memory/` 提取内容
- ✅ 自动推送到 GitHub Pages

---

## 🚀 每日自动更新

### 方式1：手动更新
```bash
cd ~/clawd/daily-journal
./update-timeline.sh
```

### 方式2：OpenClaw Cron（推荐）
```bash
# 每天晚上 22:00 自动更新
echo "0 22 * * * $HOME/clawd/daily-journal/update-timeline.sh" | crontab -
```

### 方式3：OpenClaw Heartbeat
在 `HEARTBEAT.md` 中添加：
```markdown
### 每日任务
- 生成每日总结并部署到网站
```

---

## 📝 时间线数据结构

每条记录包含：
- 📅 日期
- 📌 标题
- 📄 摘要
- 🏷️ 标签
- 💡 核心洞察
- 📖 详细内容

---

## 🎨 未来扩展

### 可以添加的功能
1. **搜索功能**：全文搜索
2. **分类标签**：AI、投资、技术、生活
3. **评论系统**：Giscus（基于 GitHub Discussions）
4. **RSS 订阅**：自动生成 RSS
5. **统计面板**：访问量、热门文章
6. **知识图谱**：可视化知识连接
7. **AI 对话**：读者可以和你的总结对话

---

## 🔐 隐私保护

### 自动过滤敏感信息
- ❌ 密码、密钥、Token
- ❌ 个人隐私信息
- ❌ 敏感财务数据
- ✅ 只发布通用内容

---

## 📊 当前状态

**网站**：✅ 已部署
**GitHub Pages**：✅ 已启用
**自动更新脚本**：✅ 已创建
**访问地址**：https://jinbo007.github.io/daily-journal/

---

## 🎯 使用流程

### 每天
1. OpenClaw 记录你的聊天内容到 `memory/YYYY-MM-DD.md`
2. 脚本自动提取关键信息
3. 生成时间线条目
4. 推送到 GitHub Pages
5. 网站自动更新

### 查看网站
访问：https://jinbo007.github.io/daily-journal/

---

**创建时间**：2026-03-09 21:45
**状态**：✅ 运行中
**下次更新**：2026-03-10 22:00（自动）
