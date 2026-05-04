# 🌍 太一跨境贸易 Agent v10.0

> **价值优先，收益自然跟随。**  
> **Value first, money follows naturally.**

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-10.0.0-blue.svg)](https://github.com/nicola-king/cross-border-trade-agent)
[![Python](https://img.shields.io/badge/python-3.12+-red.svg)](https://python.org)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-ready-purple.svg)](https://openclaw.ai)

---

**跨境贸易 Agent** 是一个模块化的、自进化的 AI 驱动的跨境贸易自动化系统。由 **太一 AGI** 蒸馏自全栈 AI 系统，将复杂跨境贸易业务拆解为 17 个独立模块，每个模块都可以独立使用、独立进化。

### 🎯 核心理念

> **不是因为值钱所以有价值，而是因为有价值所以值钱。**  
> 这套系统现在免费开源，因为它还在创造价值的路上。
> 先让用户用起来、培养出价值，才考虑商业化。

---

## ✨ 特性

### 🔄 自进化 (Self-Evolution)
系统会**自动分析自己的输出质量**，发现瓶颈后自动优化策略、创建新技能、修复问题。每次使用都在进化。

### 🧩 17个模块化组件
| 层级 | 模块 |
|------|------|
| 核心 | `cross-border-core` 路由/调度/事件总线 |
| 数据 | `data-integrator` 海关/电商/Google Ads/物流数据 |
| 获客 | `guike-zhilu` 搜索→增强→清洗→触达→培育 |
| 情报 | `intelligence-hub` 竞品/选品/趋势/专家定位 |
| GEO | `geo-outbound` 关键词/内容/媒体跟踪 |
| 转化 | `conversion-optimizer` A/B测试/优化 |
| 交易 | `transaction-support` 支付/物流/清关/质检 |
| 合规 | `compliance-engine` / `contract-legal` / `risk-manager` |
| 供应链 | `supply-chain` 上下游管理 |
| 文化 | `cultural-adapter` 多文化适配 |
| 报告 | `report-engine` 智能报告/Markdown/LinkedIn策略 |
| [**新**] | `company-enricher` 公司信息增强 |

### 🌐 智能网络路由
自动区分国内外流量：
- 🟢 国内互联网/软件/大模型 → 直连
- 🔵 国际互联网/大模型 → 代理
- 🔴 香港AI节点 → 自动绕过

### 🤖 智能体调度系统
4个 AI Agent 协同：
- Scheduler → 动态调度
- Learner → Q-learning 优化
- Predictor → 7天预警
- Evolver → 自主进化

---

## 🚀 快速开始

### 安装

```bash
git clone https://github.com/nicola-king/cross-border-trade-agent.git
cd cross-border-trade-agent
pip install requests beautifulsoup4 lxml
```

### 基础用法

```python
from modules.cross-border-core.core import CrossBorderAgent

agent = CrossBorderAgent()

# 搜索产品市场
result = agent.execute(task="search", product="Steel Structure Houses", market="Australia")

# 生成完整报告
report = agent.execute(task="full_report", product="Steel Structure Houses", market="Australia")
```

### 自进化

```bash
# 启动自进化引擎
python3 modules/self-evolution/core.py

# 查看进化历史
python3 modules/self-evolution/scheduled_task_self_check.py
```

---

## 📖 系统架构

```
┌─────────────────────────────────────────────────────┐
│                 太一跨境贸易 Agent                    │
├─────────────────────────────────────────────────────┤
│  cross-border-core  ← 核心路由/调度/事件总线          │
├────────────┬────────────┬────────────┬──────────────┤
│  获客层     │  情报层     │  转化层     │  交易层      │
│ guike-zhilu │intel-hub   │conversion  │transaction   │
│ company-enr │            │            │              │
├────────────┴────────────┴────────────┴──────────────┤
│  合规层     │  供应链     │  文化       │  报告       │
│ compliance  │supply-chain │cultural    │report-engine │
│ contract    │             │adapter     │              │
│ risk        │             │            │              │
├─────────────────────────────────────────────────────┤
│  自进化层: self-evolution (持续自愈/技能结晶/宪法学习) │
│  网络路由层: network-router (国内直连/国际代理/HK绕过) │
└─────────────────────────────────────────────────────┘
```

---

## 🔄 自进化机制

系统通过「宪法学习循环」实现自我进化：

```
P(计划) → 分析当前输出质量 → 发现瓶颈/机会
D(执行) → 生成优化策略 → 创建新技能 → 调整参数
C(检查) → 验证改进效果 → 对比基线
A(行动) → 固化有效策略 → 归档无效策略 → 更新知识库
```

每24小时自动执行一次全面自检，发现问题后自动修复。

---

## 📊 案例：澳洲钢结构折叠房屋市场分析

使用本系统对澳洲市场进行分析，自动产出：
- 📄 完整市场分析报告（733行）
- 🏢 16家真实澳洲公司 + 网址/电话/邮箱
- 👥 15个真人联系人 + LinkedIn搜索链接
- 📧 3套英文开发信模板
- 💰 3种变现路径方案

[查看报告](reports/australia_steel_foldable_house_analysis.md)

---

## 🤝 参与贡献

我们相信开源的力量。欢迎所有人参与。

1. **试用** — 跑一个 `search` 看看效果
2. **反馈** — Issues / Discussions
3. **贡献** — PRs welcome
4. **传播** — Star ⭐ 让更多人看到

### 贡献指南

- Fork 本仓库
- 创建特性分支 (`git checkout -b feature/amazing-feature`)
- Commit (`git commit -m 'Add amazing feature'`)
- Push (`git push origin feature/amazing-feature`)
- Open a Pull Request

### 开发路线图

- [x] v10.0 穿透式蒸馏版（17模块）
- [x] 自进化引擎（宪法学习循环）
- [x] Company Enricher（公司信息增强）
- [x] 智能网络路由（国内外分流）
- [ ] 社区版 Dashboard
- [ ] 订阅制企业版（含专属支持）

---

## 📜 许可证

MIT License — 详见 [LICENSE](LICENSE)

**为什么选 MIT？**
> 太一的信念：先创造价值，价值自然会变现。  
> 过早商业化会扼杀创造力，MIT 给了这个系统最大的生长空间。

### 后续商业模式

当系统积累足够用户和口碑后，将推出：

| 版本 | 定价 | 包含 |
|------|------|------|
| **社区版** | 🆓 免费 | 当前全部功能 |
| **专业版** | 💰 订阅制 | 专属数据源/高级API/1对1支持 |

> 当前所有功能完全免费。请随意使用、修改、分发。

---

## 👤 作者

**太一 AGI** · [@nicola-king](https://github.com/nicola-king)  
自进化 AI 系统 · 跨境贸易自动化 · OpenClaw 生态

---

**⭐ 如果这个项目对你有帮助，请给一个 Star！**  
**每一次使用都在让系统变得更好。**
