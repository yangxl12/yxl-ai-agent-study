用户目标 → LLM 判断下一步 → 调用 Tool → 得到结果 → 更新上下文 → 再判断 → …… → 完成任务
重点吃透 7 个概念：Tool Calling、Agent Loop、Context、Memory、Structured Output、MCP、Sub-agent。
尤其是 Agent Loop。你以前问过 Loop Engineering，这其实就是非常值得深入的方向。Agent 真正难的不是“调用一次大模型 API”，而是怎么让模型连续工作几十步，还不跑偏、不死循环、不重复调用、不把 Token 烧光。

API、SSE/WebSocket、数据库、Redis、队列、认证、Docker

| 优先级    | 后端知识                         | 为什么 Agent 开发需要   |
| --------- | -------------------------------- | ----------------------- |
| 🔥 必学   | HTTP、REST API、请求生命周期     | Agent 服务的基础        |
| 🔥 必学   | Node.js 异步、Event Loop、Stream | LLM 流式输出、并行 Tool |
| 🔥 必学   | SSE / WebSocket                  | Agent 实时返回执行过程  |
| 🔥 必学   | 数据库 + PostgreSQL 基础         | 用户、任务、Agent 状态  |
| 🔥 必学   | SQL 基础                         | 别只会 ORM              |
| 🔥 必学   | ORM（Prisma/Drizzle 任选一个）   | 实际项目开发            |
| 🔥 必学   | Redis 基础                       | Cache、任务状态、队列   |
| 🔥 必学   | Auth / JWT / Session             | 真正产品绕不开          |
| 🔥 必学   | 文件系统、进程、Shell            | Coding Agent 尤其重要   |
| ⭐ 后面学 | Queue / Worker                   | Agent 长任务、异步任务  |
| ⭐ 后面学 | Docker                           | 部署 Agent 服务         |
| ⭐ 后面学 | 日志、Tracing、错误处理          | Agent 调试非常重要      |
| 暂时不用  | 微服务、K8s、MQ 深入、分布式系统 | 现在投入产出比太低      |

做 Agent → 遇到后端问题 → 学这个问题 → 马上用进 Agent

1 Agent 基础 → 2 Context → 4 Tools/MCP → 5 Coding Agent → 7 Evaluation → 10 Multi-Agent
第 3 章 Memory/RAG 可以挑重点看。
第 6 章 Computer Use / 多模态了解。
第 8 章模型后训练、第 9 章持续进化先不要深挖
