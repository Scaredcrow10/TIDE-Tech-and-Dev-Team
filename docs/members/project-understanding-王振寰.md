# Project Understanding - 王振寰

## 1. 我对项目目标的理解

我理解这个项目是一个面向项目管理和学习小组协作的 Multi-Agent 管理系统。它的目标不是简单做一个聊天机器人，而是把 Mattermost、后端服务、数据库、前端 Dashboard 和 AI Agent 串起来，形成一个可以辅助项目管理的系统。

在第一阶段，系统应该先完成一个最小可运行的 MVP，让成员能够理解项目的整体流程，例如任务发布、任务提交、信息汇总、Agent 辅助分析和结果展示等。项目的重点是让成员从“技术学习者”逐步过渡到“项目参与者”。

## 2. 我对整体链路的理解

我理解的系统整体链路大概是：

```text
Mattermost / 前端页面
↓
后端 API
↓
数据库
↓
AI Agent
↓
结果汇总与展示
```

其中，Mattermost 可以作为协作入口，例如通过 Slash Command、Webhook 或 Bot 接收用户操作；后端负责处理请求和业务逻辑；数据库负责保存项目、任务、用户、提交内容和评估结果；AI Agent 负责对任务或提交内容进行总结、分析或生成建议；前端 Dashboard 负责把系统状态可视化展示出来。

## 3. 我对 MVP 范围的理解

我认为第一阶段 MVP 不需要做得很复杂，应该先跑通一个完整闭环。比如：

1. 用户可以通过 Mattermost 或前端创建任务；
2. 后端能够接收请求并保存数据；
3. 数据库能够持久化任务或提交记录；
4. 前端能够展示任务状态；
5. Agent 能够对任务或提交内容做简单总结；
6. 系统能够把结果返回给用户或展示在页面中。

我理解 MVP 的重点不是功能数量多，而是证明核心流程可以跑通：

```text
入口操作 → 后端处理 → 数据保存 → Agent 分析 → 结果展示
```

## 4. 我需要学习的技术内容

根据目前的项目要求，我觉得自己需要重点学习以下内容：

* Git 协作：branch、commit、push、pull request、review；
* Mattermost 集成：Slash Command、Webhook、Bot Account；
* 后端开发：REST API、NestJS、接口设计；
* 数据库：PostgreSQL、Prisma、基础数据建模；
* 前端开发：React、TypeScript、Dashboard 页面和 API 调用；
* AI Agent：LLM API、Prompt、Tool Calling、结构化输出；
* 本地部署：Docker、Docker Compose、环境变量配置。

## 5. 我已经做过的初步实践

在完成本次作业前，我尝试做了一个简化练习项目，用来理解类似的技术链路。这个练习项目中，我使用 Next.js 做了一个简单前端 Dashboard，用 NestJS 写了后端 API，用 PostgreSQL 和 Prisma 保存任务数据，并用 Docker Compose 启动数据库。

此外，我也模拟了 Mattermost Slash Command 接口，实现了通过命令创建任务和查看任务 summary，并加入了简单的 token 校验。通过这个练习，我对“前端 → 后端 → 数据库 → 协作平台入口”的基本流程有了更具体的理解。

## 6. 我目前的疑问

目前我还有一些问题需要后续继续明确：

1. 第一阶段是否必须接入真实 Mattermost，还是可以先用模拟请求完成？
2. 用户身份和权限是否需要在 MVP 阶段实现？
3. 数据库中的核心对象应该包括哪些，例如 Project、Task、User、Submission、Evaluation？
4. Agent 的输出是否需要固定 JSON 格式？
5. 前端 Dashboard 第一阶段需要做到多复杂？
6. 最终验收更看重系统可运行，还是更看重项目理解和协作流程？

## 7. 我的下一步计划

接下来我计划先继续熟悉 Git 协作流程，然后重点学习 Mattermost 接入、NestJS 后端 API、PostgreSQL 数据建模和基础 Agent 调用方式。我的目标是先理解项目整体链路，并能参与基础模块的实现，而不是一开始就追求复杂功能。
