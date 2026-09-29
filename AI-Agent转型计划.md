# AI Agent 开发转型计划

## 1. 转型目标

基于现有 **6+ 年前端开发经验**，向以下岗位转型：

- AI Agent 应用工程师
- AI Agent 全栈工程师
- AI Native 应用工程师
- AI 工具 / 客户端工程师
- Agent Harness 工程师

核心思路不是从零转行，而是：

> 前端工程能力 + Agent 能力 + 必要的后端能力

---

## 2. 学习原则

### 不追求“全部学完再做项目”

采用 **边学边做** 的方式：

1. 先建立 Agent 整体认知
2. 学 Agent Harness 核心机制
3. 补 Agent 开发真正需要的后端知识
4. 同时开始做自己的完整项目
5. 项目做到一定程度后就开始投简历和面试

---

## 3. 学习路线

### 第一阶段：Agent 基础认知（约 1 周）

主线：`bojieli/ai-agent-book`

重点理解：

- Agent Loop
- Tool Calling
- Context
- Memory
- RAG
- Planning
- SubAgent
- MCP
- Eval

目标：搞清楚每个概念 **解决什么问题**，不追求背 API。

---

### 第二阶段：Agent Harness 实战（约 2 周）

主线：`ryzqi/learn-agent`

重点掌握：

- Agent Loop
- Tool Registry
- Permission
- Hooks
- Planning / Todo
- Context Compaction
- Memory
- SubAgent
- Task / Background Task
- Worktree
- MCP

学习方式：每学一个模块，都自己增加或修改功能，不只看代码。

例如自己实现：

- 文件搜索 Tool
- Git Tool
- Shell Tool
- Tool 超时 / 重试
- 权限确认
- Context 压缩
- SubAgent

`shareAI-lab/learn-claude-code` 作为补充资料，不需要完整再刷一遍。

---

## 4. 补齐必要后端能力（约 2~3 周，穿插进行）

不需要先成为传统后端工程师，只补 Agent 项目真正需要的部分。

重点学习：

- Node.js / Python 基础后端
- HTTP / REST API
- async / await 与并发
- PostgreSQL / MySQL CRUD
- 数据库事务
- Redis
- 后台任务 / 任务队列
- SSE 流式输出
- 登录认证 / 权限
- Docker
- 日志、Trace、错误处理

建议：

- 前期继续使用熟悉的 TypeScript / Node.js
- 后期补 Python + FastAPI + Pydantic + asyncio

遇到具体陌生知识，再用 `/teach` 针对性学习，不单独花大量时间系统刷后端课程。

---

## 5. 做一个真正能拿去面试的 Agent 项目

不要只做一个“聊天机器人”。

建议项目方向：

## AI Workspace Agent / Coding Workspace Agent

核心流程：

```text
读取项目 / 文档
    ↓
理解上下文
    ↓
制定执行计划
    ↓
调用 File / Git / Shell / Search 等工具
    ↓
执行任务
    ↓
必要时人工确认
    ↓
SubAgent 并行处理
    ↓
Context 压缩
    ↓
任务恢复 / Memory
    ↓
输出最终结果
```

项目逐渐加入：

- Tool Calling
- Permission
- MCP
- RAG
- Memory
- SubAgent
- SSE
- PostgreSQL
- Redis
- Checkpoint
- Trace
- Eval
- 错误重试
- Token / 成本统计

前端界面继续发挥自己的优势，做成一个真正可使用的产品，而不是 Demo。

---

## 6. 8 周执行节奏

| 时间 | 主要任务 |
|---|---|
| 第 1 周 | 快速学习 `ai-agent-book`，建立知识地图 |
| 第 2~3 周 | 主攻 `learn-agent`，边学边改代码 |
| 第 3~5 周 | 补 Node/Python、数据库、Redis、SSE、Docker 等后端能力 |
| 第 4 周开始 | 正式开发自己的 Agent 项目 |
| 第 5~6 周 | 加入 MCP、RAG、Memory、SubAgent、Checkpoint 等能力 |
| 第 6~8 周 | 完善项目、README、架构图、Demo、简历项目描述 |
| 第 7 周开始 | 开始投递简历和面试，根据面试反馈继续补知识 |

---

## 7. 求职定位

不要把自己包装成：

> 没有后端经验、刚学 AI 的前端新人。

更适合的定位是：

> 6+ 年 Web / 客户端研发经验，长期使用 TypeScript / Vue / Electron，正在向 AI Agent 工程化方向转型，具备 Agent Harness、Tool Calling、MCP、RAG、Memory、SubAgent，以及 Node/Python 后端开发能力，并有完整 Agent 项目实践。

---

## 8. 当前最重要的事情

现在不需要继续搜更多教程。

接下来重点只有三件事：

1. **学懂 Agent 的核心运行机制**
2. **补够真实 Agent 项目需要的后端能力**
3. **完成一个真正能拿去面试的 Agent 项目**

最终目标不是“学完 AI Agent”，而是达到：

> 能独立设计、开发、调试和讲清楚一个完整的 Agent 系统。
