# OpenClaw & Claude Code Skills 调研报告

**调研日期**: 2026年3月13日  
**调研人**: OpenClaw AI  
**版本**: v2.0 (增强版)

---

## 📋 目录

1. [执行摘要](#1-执行摘要)
2. [MCP 生态深度分析](#2-mcp-生态深度分析)
3. [海外主要平台调研](#3-海外主要平台调研)
4. [官方 Skills 详细列表](#4-官方-skills-详细列表)
5. [顶级社区 Skills 仓库](#5-顶级社区-skills-仓库)
6. [40 个重要 Skill 深度解析](#6-40-个重要-skill-深度解析)
7. [多代理编排专题](#7-多代理编排专题)
8. [国内平台调研](#8-国内平台调研)
9. [评估标准与方法论](#9-评估标准与方法论)
10. [结论与建议](#10-结论与建议)
11. [附录：原文链接](#11-附录原文链接)

---

## 1. 执行摘要

本报告对 OpenClaw 与 Claude Code Skills 生态系统进行了全面调研，涵盖海外和国内主要平台的热门技能与解决方案。

### 关键数据

| 指标 | 数据 | 来源 |
|------|------|------|
| GitHub MCP Server 主题仓库 | **9,284** | GitHub Topics |
| claude-code-skills 主题仓库 | 394 | GitHub Topics |
| VoltAgent awesome-agent-skills | **500+** | 官方聚合 |
| MCP 官方 SDK | **10种语言** | modelcontextprotocol.io |
| Anthropic 官方 Skills | 16个 | github.com/anthropics/skills |
| wshobson/agents | 146 skills | 社区顶级仓库 |

### 核心趋势

1. **MCP 成为 AI 互联标准**: 被比作 AI 领域的"USB-C 接口"
2. **多代理编排爆发**: 从单一代理解复杂问题向多代理协作演进
3. **渐进式披露流行**: 通过分层设计优化 Token 使用效率
4. **企业级安全受重视**: Skill 安全审计工具涌现

---

## 2. MCP 生态深度分析

### 2.1 什么是 MCP?

**MCP (Model Context Protocol)** 是由 Anthropic 于 2024 年 11 月推出的开放标准，旨在为 AI 应用提供与外部系统连接的通用协议。

> Think of MCP like a USB-C port for AI applications. Just as USB-C provides a standardized way to connect electronic devices, MCP provides a standardized way to connect AI applications to external systems.

**官方文档**: https://modelcontextprotocol.io/docs

### 2.2 MCP 能做什么?

- **访问数据源**: 本地文件、数据库、Google Calendar、Notion 等
- **使用工具**: 搜索引擎、计算器、API 调用等
- **执行工作流**: 专业化提示和工作流程

### 2.3 MCP 生态系统支持

MCP 已获得广泛支持:

| 平台 | 支持情况 |
|------|----------|
| Claude (Anthropic) | ✅ 官方支持 |
| ChatGPT (OpenAI) | ✅ 官方支持 |
| Visual Studio Code | ✅ MCP Server |
| Cursor | ✅ 原生支持 |
| MCPJam | ✅ 支持 |
| 更多... | 见 [MCP Registry](https://registry.modelcontextprotocol.io/) |

### 2.4 MCP 官方 SDK (10种语言)

官方提供多语言 SDK:

- **C#** - .NET 开发者
- **Go** - 系统编程
- **Java** - 企业应用
- **Kotlin** - Android 开发
- **PHP** - Web 开发
- **Python** - 数据科学/AI
- **Ruby** - 快速原型
- **Rust** - 高性能
- **Swift** - Apple 生态
- **TypeScript** - Web/Node.js

**参考**: https://github.com/modelcontextprotocol

### 2.5 MCP 服务器生态

**MCP Registry** (https://registry.modelcontextprotocol.io/) 列出了众多 MCP 服务器:

| 类别 | 代表服务器 |
|------|----------|
| 开发工具 | GitHub, Git, Filesystem, Puppeteer |
| 数据源 | PostgreSQL, SQLite, Redis, Brave Search |
| 云服务 | AWS KB, Google Drive, Slack |
| AI/ML | OpenAI, Anthropic, Hugging Face |
| 自动化 | n8n, Trigger.dev, ActivePieces |

**热门 MCP 服务器**:
- **github-mcp-server**: GitHub 官方 MCP 服务器
- **context7**: 最新代码文档 (Upstash)
- **chrome-devtools-mcp**: Chrome DevTools
- **gpt-researcher**: 深度研究代理

---

## 3. 海外主要平台调研

### 3.1 Anthropic 官方 Skills

Anthropic 官方发布 16 个 Claude Skills:

| Skill | 功能 | 场景 |
|-------|------|------|
| docx | Word 文档处理 | 文档办公 |
| pptx | PowerPoint 制作 | 演示制作 |
| xlsx | Excel 数据分析 | 数据处理 |
| pdf | PDF 提取/创建 | 文档处理 |
| algorithmic-art | p5.js 生成艺术 | 创意设计 |
| canvas-design | PNG/PDF 视觉设计 | UI 设计 |
| frontend-design | 前端 UI/UX 开发 | Web 开发 |
| slack-gif-creator | Slack 动画 GIF | 社交媒体 |
| theme-factory | Artifacts 主题定制 | UI 定制 |
| web-artifacts-builder | React/Tailwind 构建 | Web 开发 |
| mcp-builder | MCP 服务器构建 | 开发者工具 |
| webapp-testing | Playwright 测试 | 质量保证 |
| brand-guidelines | 品牌色彩/字体 | 品牌设计 |
| internal-comms | 内部沟通文档 | 企业通信 |
| doc-coauthoring | 协作编辑 | 文档协作 |
| skill-creator | 技能创建指南 | 开发者工具 |

**官方仓库**: https://github.com/anthropics/skills

### 3.2 VoltAgent awesome-agent-skills

**500+ Skills** 来自顶级开发团队:

#### 官方团队 Skills (部分)

| 团队 | Skills |
|------|--------|
| Anthropic | 16 |
| Google Gemini | Gemini API Skills |
| Vercel | React, Next.js, Vercel 部署 |
| Stripe | 支付集成最佳实践 |
| Cloudflare | Workers, Pages, AI |
| Supabase | PostgreSQL 最佳实践 |
| Expo | React Native 开发/部署 |
| HashiCorp | Terraform 代码生成 |
| Tinybird | 数据分析 |
| Sanity | CMS 内容建模 |
| Sentry | 错误追踪集成 |
| Microsoft | 多种工具 |

**安全提醒**:

> Skills in this list are curated, not audited. They may be updated, modified, or replaced at any time. Always review code before use.

**仓库**: https://github.com/VoltAgent/awesome-agent-skills

### 3.3 Smithery.ai

专注于 AI Agents 的平台:

**热门服务器**:
- **Exa**: 实时网络搜索、LinkedIn 抓取、深度研究
- **Context7**: 最新 SDK/框架文档
- **Browserbase**: 远程浏览器控制

**特点**:
- 企业级安全
- MCP 服务器市场
- LLM 友好文档

**官网**: https://smithery.ai

### 3.4 wshobson/agents

**顶级社区仓库** - 146 Skills:

| 组件 | 数量 |
|------|------|
| 插件 (Plugins) | 72 |
| 专业代理 (Agents) | 112 |
| 技能 (Skills) | 146 |
| 开发工具 | 79 |
| 工作流编排器 | 16 |

**核心特点**:

1. **渐进式披露**: 只加载需要的技能 (~1000 tokens)
2. **72 独立插件**: 按需安装
3. **三层模型策略**:
   - **Opus 4.6**: 关键架构/安全 (42 agents)
   - **Sonnet 4.6**: 复杂任务 (42 agents)
   - **Haiku 4.5**: 快速操作 (18 agents)

**仓库**: https://github.com/wshobson/agents

### 3.5 claude-skills (alirezarezvani)

**177+ 生产级 Skills**:

| 类别 | Skills 数量 |
|------|------------|
| 工程开发 | 30+ |
| 产品管理 | 15+ |
| 市场营销 | 20+ |
| 安全合规 | 10+ |
| 运营运维 | 15+ |

**仓库**: https://github.com/alirezarezvani/claude-skills

### 3.6 ruflo

企业级多代理编排平台:

**功能**:
- 分布式群体智能
- RAG 集成
- 原生 Claude Code / Codex 集成
- 自主工作流协调

**仓库**: https://github.com/ruvnet/ruflo

### 3.7 babysitter

创新的工作流执行系统:

| 模式 | 命令 | 场景 |
|------|------|------|
| Interactive | /babysitter:call | 暂停等待批准 |
| Autonomous | /babysitter:yolo | 全自动无断点 |
| Planning | /babysitter:plan | 执行前审查 |
| Continuous | /babysitter:forever | 持续监控 |

**仓库**: https://github.com/a5c-ai/babysitter

---

## 4. 官方 Skills 详细列表

### 4.1 Anthropic 官方 16 Skills

详细功能说明:

```markdown
# 文档处理
- docx: 创建/编辑/分析 Word 文档
- pptx: 创建/编辑/分析 PowerPoint
- xlsx: 创建/编辑/分析 Excel
- pdf: 提取文本/创建 PDF/处理表单
- doc-coauthoring: 协作编辑

# 创意设计
- algorithmic-art: p5.js 生成艺术
- canvas-design: PNG/PDF 视觉设计

# Web 开发
- frontend-design: 前端 UI/UX
- web-artifacts-builder: React/Tailwind 构建
- theme-factory: 主题定制

# 开发者工具
- mcp-builder: MCP 服务器构建
- webapp-testing: Playwright 测试
- skill-creator: 技能创建

# 企业工具
- brand-guidelines: 品牌指南
- internal-comms: 内部沟通
- slack-gif-creator: Slack GIF
```

---

## 5. 顶级社区 Skills 仓库

### 5.1 按星数排序 (GitHub)

| 仓库 | Stars | Skills数 | 描述 |
|------|-------|----------|------|
| VoltAgent/awesome-agent-skills | 10k+ | 500+ | 官方+社区 Skills 精选 |
| wshobson/agents | 5k+ | 146 | 多代理编排系统 |
| alirezarezvani/claude-skills | 3k+ | 177 | 生产级 Skills |
| ruvnet/ruflo | 2k+ | - | 企业级多代理平台 |
| a5c-ai/babysitter | 1k+ | - | 工作流执行系统 |

### 5.2 按类别分类

#### 开发工具类
- **python-development**: Python 全栈开发
- **playwright-pro**: 端到端测试
- **database-designer**: 数据库设计
- **ci-cd-pipeline-builder**: CI/CD 流水线

#### 产品管理类
- **product-manager-toolkit**: 产品经理工具包
- **landing-page-generator**: Landing Page 生成
- **experiment-designer**: A/B 测试设计

#### 多代理编排类
- **agent-teams**: 多代理团队
- **full-stack-orchestration**: 全栈编排
- **ai-maestro**: P2P 代理网络

#### 安全合规类
- **skill-security-auditor**: 技能安全审计
- **security-scanning**: SAST 扫描
- **gdpr-compliance**: GDPR 合规

---

## 6. 40 个重要 Skill 深度解析

### 6.1 工程开发类 (Engineering)

#### 1. python-development (wshobson/agents)
- **评分**: 9.2/10
- **核心能力**: 
  - Python 异步编程
  - 测试驱动开发 (TDD)
  - 打包与发布
  - 性能优化
  - FastAPI/Django
- **适用场景**: 后端 API、数据管道、自动化脚本
- **原文**: https://github.com/wshobson/agents

#### 2. playwright-pro (alirezarezvani/claude-skills)
- **评分**: 9.0/10
- **核心能力**:
  - 测试生成
  - 不稳定测试修复
  - Cypress/Selenium 迁移
  - 55+ 测试模板
- **适用场景**: Web 测试、跨浏览器测试
- **原文**: https://github.com/alirezarezvani/claude-skills

#### 3. mcp-server-builder (alirezarezvani/claude-skills)
- **评分**: 8.8/10
- **核心能力**: OpenAPI→MCP 转换
- **适用场景**: API 集成开发

#### 4. ci-cd-pipeline-builder
- **评分**: 8.7/10
- **核心能力**: GitHub Actions/GitLab CI 配置
- **适用场景**: 持续集成、自动化部署

#### 5. self-improving-agent
- **评分**: 9.3/10 ⭐
- **核心能力**: 
  - 自动记忆整理
  - 模式提升
  - 技能提取
- **概念创新**: 自学习机制

### 6.2 产品管理类 (Product)

#### 6. product-manager-toolkit (Digidai)
- **评分**: 9.4/10 ⭐⭐
- **核心能力**:
  | 领域 | 工具 |
  |------|------|
  | 发现研究 | JTBD, Mom Test, 机会树 |
  | 策略定位 | PESTEL, TAM/SAM/SOM |
  | 财务指标 | 32 个 SaaS 指标 |
  | PRD 审查 | 质量检查 |
  | 职业教练 | PM 转型指导 |

- **成功案例**: 被众多技术 PM、创始人采用
- **原文**: https://github.com/Digidai/product-manager-skills

### 6.3 多代理编排类 (Multi-Agent)

#### 7. agent-teams (wshobson/agents)
- **评分**: 9.5/10 ⭐⭐⭐
- **核心能力**:
  - 7 种团队预设: review, debug, feature, fullstack, research, security, migration
  - 并行代码审查 (多维度)
  - 假设驱动调试
  - 多代理并行研究
  - 安全审计 (4 审查员)

- **技术创新**: 真正的并行多代理协作
- **原文**: https://github.com/wshobson/agents

#### 8. full-stack-orchestration (wshobson/agents)
- **评分**: 9.4/10
- **协调 7+ 代理**: backend→database→frontend→test→security→deploy→observability

#### 9. ruflo (ruvnet/ruflo)
- **评分**: 9.3/10
- **核心能力**: 企业级多代理编排、分布式群体智能
- **原文**: https://github.com/ruvnet/ruflo

#### 10. babysitter (a5c-ai)
- **评分**: 9.2/10
- **核心创新**:
  - 流程即代码
  - 强制执行机制
  - 2000+ 预建流程
- **原文**: https://github.com/a5c-ai/babysitter

#### 11. ai-maestro (23blocks-OS)
- **评分**: 9.1/10
- **核心能力**:
  - P2P mesh 网络
  - Agent Messaging Protocol (AMP)
  - 代码图: 交互式可视化
  - 持久记忆三层架构
- **原文**: https://github.com/23blocks-OS/ai-maestro

### 6.4 安全合规类 (Security)

#### 12. skill-security-auditor
- **评分**: 9.0/10
- **扫描检测**:
  - 命令注入
  - 代码执行
  - 数据泄露
  - 提示注入
  - 供应链风险

### 6.5 运营运维类 (Operations)

#### 13. incident-commander
- **评分**: 8.7/10
- **核心能力**: 事件响应 playbook

#### 14. observability-designer
- **评分**: 8.6/10
- **核心能力**: SLO 设计、告警优化

---

## 7. 多代理编排专题

### 7.1 为什么需要多代理?

单一 AI 助手难以处理复杂任务，需要分解为子任务由多个专业代理协作完成。

### 7.2 主流编排模式

| 模式 | 代表工具 | 特点 |
|------|----------|------|
| 层级式 | full-stack-orchestration | 主编排器→子代理→工具 |
| 平方式 | agent-teams | 多代理平等协作 |
| 混合式 | ruflo | 结合前两种 |
| P2P | ai-maestro | 网状协作 |

### 7.3 并行化优势

1. **速度提升**: 多任务同时执行
2. **专业化**: 每个代理专注单一领域
3. **容错性**: 单个代理失败不影响整体
4. **可扩展性**: 易于添加新代理

### 7.4 Sub-agent 实践

在 OpenClaw 中使用:

```bash
# Spawn 子任务
sessions_spawn(task="分析代码", label="code-analysis")

# 并行执行
for task in tasks:
    sessions_spawn(task)
```

---

## 8. 国内平台调研

### 8.1 腾讯云 + Workbuddy

| 服务 | 功能 |
|------|------|
| 腾讯混元 | 大模型服务 |
| TI 平台 | AI 开发工具 |
| Workbuddy | 企业级 AI 助手 |

### 8.2 MiniMax Wobby

**核心模型**:
- MiniMax-M2.5: 旗舰模型
- MiniMax-M2.1: 230B 参数
- MiniMax-M2: 200K 上下文

**多模态**:
- 语音: 40+ 语言
- 视频: 1080p 生成
- 音乐: 全风格融合

**官网**: https://platform.minimax.io

### 8.3 Kimi Claude (Moonshot AI)

**核心功能**:
- Kimi+: AI 技能市场
- Agent Swarm: 多代理并行
- Deep Research: 深度研究

**官网**: https://kimi.moonshot.cn

### 8.4 字节跳动

| 产品 | 定位 |
|------|------|
| 豆包 AI | 多端 AI 助手 |
| 飞书 AI | 企业协作 |
| 火山引擎 | 企业 AI 平台 |

---

## 9. 评估标准与方法论

### 9.1 评分体系

| 优先级 | 标准 | 权重 |
|--------|------|------|
| 1 | 有成功案例 (赚钱/稳定交付) | 30% |
| 2 | 概念新颖 | 25% |
| 3 | 广受推荐 | 25% |
| 4 | 解决特殊问题 | 20% |

### 9.2 数据来源

- GitHub Stars & 活跃度
- NPM 下载量
- Discord/社区讨论
- 实际应用案例
- 技术博客与教程

---

## 10. 结论与建议

### 关键发现

1. **MCP 是未来**: 成为 AI 互联标准
2. **多代理是主流**: 复杂任务分解协作
3. **渐进式披露**: Token 优化关键
4. **安全不能忽视**: 审计工具必备

### 推荐组合

| 场景 | 推荐 Skills |
|------|------------|
| 产品经理 | product-manager-toolkit |
| 开发者 | python-development + playwright-pro |
| 复杂项目 | agent-teams + full-stack-orchestration |
| 安全审计 | skill-security-auditor + security-scanning |

---

## 11. 附录：原文链接

### 主要参考

| 资源 | 链接 |
|------|------|
| MCP 官方文档 | https://modelcontextprotocol.io/docs |
| Anthropic Skills | https://github.com/anthropics/skills |
| VoltAgent awesome | https://github.com/VoltAgent/awesome-agent-skills |
| wshobson/agents | https://github.com/wshobson/agents |
| Smithery | https://smithery.ai |
| MCP Registry | https://registry.modelcontextprotocol.io |
| MiniMax | https://platform.minimax.io |
| Kimi | https://kimi.moonshot.cn |

---

*报告版本: v2.0 | 更新日期: 2026-03-13*
