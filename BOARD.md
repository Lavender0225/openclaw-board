# BOARD.md - 任务看板

> 最后更新：2026-04-08 16:00

## 任务状态

### 进行中
| 任务 | Agent | 状态 | 开始时间 |
|------|-------|------|----------|
| 4B MLX embedding 接入 | 总管 | 🟡 P3 待验证 | 2026-04-06 |
| Obsidian 深度调研 | 调研牛马 | 🔄 进行中 | 2026-04-07 |
| Claude Code 源码文章学习 | 学习牛马 | 🔄 进行中 | 2026-04-07 |
| 看板自动从 memory 汇总更新机制 | 待分配 | 🟡 待设计 | 2026-04-08 |

### 今日完成（4/8）
| 任务 | Agent | 完成时间 | 说明 |
|------|-------|----------|------|
| ✅ 飞书新闻超链接修复 | 干活牛马 | 08:08 | Markdown链接→裸URL，飞书可点击 |
| ✅ 废弃新闻脚本清理 | 干活牛马 | 08:13 | 删除8个无用脚本（trash可恢复） |
| ✅ 知识库 Web 系统上线 | 干活牛马 | 13:15 | Express+markdown-it，公网可访问 |
| ✅ Web 登录修复 | 干活牛马 | 13:27 | helmet upgrade-insecure-requests 导致静默失败 |
| ✅ Web 样式优化 v3 | 干活牛马 | 13:40 | CSS外置+亮暗主题切换+GitHub风格 |
| ✅ 多格式支持 | 干活牛马 | 13:53 | 图片预览/PDF内嵌/JSON高亮 |
| ✅ launchd 开机自启+崩溃恢复 | 干活牛马 | 14:05 | 5秒自动拉起，已实测 |
| ✅ 知识库交叉引用补全 | 干活牛马 | 14:23 | 20%→70%（105页更新），超额完成 |
| ✅ 失效链接修复 | 干活牛马 | 14:25 | 5个失效[[]]引用修复，0死链 |
| ✅ 教程学习笔记归位 | 干活牛马 | 14:45 | 5个文件从summaries移入教程目录 |
| ✅ linkify 中文路径误判修复 | 干活牛马 | 14:55 | 关闭linkify，修复20+个假链接 |
| ✅ index.md 空格链接修复 | 干活牛马 | 15:01 | 50个含空格路径编码为%20 |
| ✅ Mermaid 图渲染支持 | 干活牛马 | 15:10 | 引入mermaid.js CDN，跟随主题切换 |
| ✅ 教程配图归位 | 干活牛马 | 15:15 | entities/图表+配图 移入教程目录 |
| ✅ index.md 文件夹分层 | 干活牛马 | 15:20 | generate-index.js 改为按目录分组 |
| ✅ 目录树状态持久化 | 干活牛马 | 15:50 | sessionStorage保存展开/滚动状态 |
| ✅ JSON亮色模式修复 | 干活牛马 | 14:42 | 代码块亮色背景+深色文字 |
| ✅ 新闻报告超链接修复 | 总管 | 08:18 | generate_markdown() 标题改为 [title](url) |
| ✅ Cron 任务批量修复（9个error） | 总管 | 08:22 | 6个channel问题+1个target+3个timeout |
| ✅ qwen3-embedding:0.6b 生效验证 | 总管 | 08:20 | 本 session memory_search 已确认生效 |
| ✅ 知识库 index 更新 | 总管 | 08:23 | 114 wiki + 100 raw |
| ✅ Agent 配置瘦身 M1+M2 | 干活牛马 | 10:50 | 4个Agent瘦身65-72% |

### 近期完成（4/3 - 4/7）
| 任务 | Agent | 完成时间 | 说明 |
|------|-------|----------|------|
| ✅ 公众号搜索工具调研+安装 | 总结牛马 | 2026-04-07 | wechat-articles skill 安装+安全审查 |
| ✅ Agent 专属频道不回复修复 | 总管 | 2026-04-07 | 5 个 Agent AGENTS.md 加专属频道规则 |
| ✅ 36kr 新闻源修复 | 总管 | 2026-04-07 | 网页爬虫→RSS |
| ✅ 代理环境变量统一 | 总管 | 2026-04-07 | ~/.zshenv + start.sh |
| ✅ 知识库 Wiki 化迁移 | 总管+干活 | 2026-04-06 | 237 文件 |
| ✅ Embedding 模型切换 | 总管 | 2026-04-06 | nomic→qwen3-embedding:0.6b |
| ✅ 新闻推送防重发 | - | 已有 | send-to-group.py 内置 MD5+1h 冷却 |

### 历史完成
| 任务 | Agent | 完成时间 |
|------|-------|----------|
| Claude Code vs OpenCode 对比 | 调研+干活 | 2026-04-01 |
| 内网 skill 仓库方案调研 | 调研+干活 | 2026-03-30 |
| 教程第一篇：Agent 基础概念 | 全体 | 2026-03-19 |
| Self-Improve 系统全套 | 干活+总结 | 2026-03-15 |

---

## Agent 状态

| Agent | 角色 | 专属频道 | 最后活跃 | 当前任务 |
|-------|------|----------|----------|----------|
| 总管 (main) | 协调调度 | - | 2026-04-08 | 知识库整理指挥 |
| 干活牛马 (worker) | 代码执行 | #干活 | 2026-04-08 16:00 | 知识库Web系统+交叉引用+配置瘦身 |
| 调研牛马 (research) | 技术调研 | #调研 | 2026-04-07 21:46 | Obsidian 深度调研 |
| 学习牛马 (learning) | 学习整理 | #学习 | 2026-04-07 16:19 | Claude Code 源码学习 |
| 设计牛马 (designer) | 方案设计 | #设计 | 2026-04-07 16:16 | 频繁 timeout |
| 总结牛马 (summarizer) | 总结汇报 | #总结 | 2026-04-08 11:15 | 巡检测试 |

## Cron 任务（4/8 修复后）
| 任务 | 频率 | Agent | 状态 | 修复说明 |
|------|------|-------|------|----------|
| 早报 | 每天 07:00 | summarizer | ✅ | timeout→600s |
| 新闻 08:00 | 每天 08:00 | summarizer | ✅ | delivery→none |
| 新闻 12:00 | 每天 12:00 | summarizer | ✅ | delivery→none |
| 新闻 18:00 | 每天 18:00 | summarizer | ✅ | delivery→none |
| 日报 | 每天 19:00 | summarizer | ✅ | 正常 |
| Self-Improve 每日分析 | 每天 22:00 | summarizer | ✅ | 加飞书 target |
| Self-Improve LLM 分析 | 每 6h | summarizer | ✅ | delivery→none |
| 夜间巡检 | 每天 01:00 | worker | ✅ | 正常 |
| 用户画像更新 | 每天 02:00 | research | ✅ | delivery→none |
| Session 清理 | 每天 03:00 | worker | ✅ | delivery→none |
| 知识库健康检查 | 每周日 03:00 | worker | ✅ | 正常 |
| 看板自动更新 | 每 30min | worker | ✅ | timeout→300s |
| 知识库→GitHub | 每小时 | worker | ✅ | timeout→300s |

---

## 已知问题
| 问题 | 优先级 | 状态 |
|------|--------|------|
| Discord MarsLink 代理不稳定 | P2 | 监控中（自动重连正常） |
| 决策卡片 55 张废卡待清理 | P3 | 待处理 |
| 看板 cron 只检测变更不主动更新内容 | P2 | 需设计自动汇总机制 |
| 4B MLX embedding ollama 优先级冲突 | P3 | 待解决 |
| HN RSS 偶尔抓取失败（超时） | P3 | 待优化 |

## 知识库 Web 系统
| 项 | 内容 |
|-----|------|
| 地址 | http://112.126.68.77:25555 |
| 代码 | ~/.openclaw/knowledge-web/ |
| 管理 | manage.sh start/stop/restart/status/logs |
| 自启 | launchd (com.openclaw.knowledge-web) |
| 文档 | wiki/projects/knowledge-web/README.md |
