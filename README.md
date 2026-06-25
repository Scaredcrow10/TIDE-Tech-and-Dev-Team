# TIDE Tech and Dev Team 学习仓库

这是 TIDE Tech and Dev Team 的项目学习与协作练习仓库。当前阶段的重点不是追求代码量，而是让每位成员熟悉真实工程协作中的基本流程：理解项目目标、创建分支、提交文档、发起 Pull Request，并根据 Review 意见继续修改。

## 当前作业

- [作业 1：Git 协作与项目理解作业](docs/assignments/assignment-1-git-collaboration.md)
- 建议完成时间：2026-06-24 至 2026-06-26
- 成员提交目录：`docs/members/`
- 可复制模板：`docs/templates/project-understanding-template.md`

## 成员需要完成什么

1. Fork 或 clone 本仓库。
2. 基于 `main` 创建个人开发分支，格式为 `learn/你的姓名或昵称`。
3. 在 `docs/members/` 新增个人学习记录文档，格式为 `project-understanding-你的姓名.md`。
4. 在文档中写出自己对项目目标、整体链路、MVP 范围的理解，也可以写真实疑问。
5. 提交 Commit，格式为 `docs: add project understanding by 你的姓名`。
6. 向 `main` 发起 Pull Request，标题格式为 `[学习作业1] 项目理解文档 - 你的姓名`。
7. 根据 Review 意见修改并更新 PR。

## 推荐本地命令

```bash
git clone https://github.com/Scaredcrow10/TIDE-Tech-and-Dev-Team.git
cd TIDE-Tech-and-Dev-Team
git checkout main
git pull origin main
git checkout -b learn/你的姓名或昵称
```

完成文档后：

```bash
git add docs/members/project-understanding-你的姓名.md
git commit -m "docs: add project understanding by 你的姓名"
git push origin learn/你的姓名或昵称
```

然后在 GitHub 页面发起 Pull Request。

## 仓库结构

```text
.
├── README.md
├── CONTRIBUTING.md
├── docs
│   ├── assignments
│   │   └── assignment-1-git-collaboration.md
│   ├── members
│   │   └── .gitkeep
│   └── templates
│       └── project-understanding-template.md
└── .github
    └── pull_request_template.md
```

## 给管理者的 Review 建议

Review 时优先看这些点：

- 文件是否放在 `docs/members/` 下；
- 文件名、分支名、Commit 信息、PR 标题是否符合要求；
- 文档是否包含项目目标、整体链路、MVP 范围、个人疑问等内容；
- 是否完成至少一轮 Review 交互。
