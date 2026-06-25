# 作业 1：Git 协作与项目理解作业

建议完成时间：2026-06-24 至 2026-06-26

## 目标

检验成员是否具备基本工程协作能力，并帮助成员理解项目整体目标、协作链路和当前 MVP 范围。

本次作业的重点包括：

- 能够正确使用分支完成个人修改；
- 能够按规范提交 Commit；
- 能够发起 Pull Request；
- 能够在 Review 中沟通和修改；
- 能够用自己的话说明对项目的理解与疑问。

## 任务内容

每位成员需要完成以下事项。

### 1. 获取仓库

可以选择 Fork 或 clone 项目学习仓库。

仓库地址：

```text
https://github.com/Scaredcrow10/TIDE-Tech-and-Dev-Team
```

如果是直接 clone：

```bash
git clone https://github.com/Scaredcrow10/TIDE-Tech-and-Dev-Team.git
cd TIDE-Tech-and-Dev-Team
```

### 2. 创建个人分支

基于 `main` 分支创建个人开发分支。

分支命名格式：

```text
learn/你的姓名或昵称
```

示例：

```bash
git checkout main
git pull origin main
git checkout -b learn/zhangsan
```

### 3. 新增个人学习记录文档

在 `docs/members/` 目录下新增一份个人学习记录文档。

文件命名格式：

```text
project-understanding-你的姓名.md
```

示例：

```text
docs/members/project-understanding-zhangsan.md
```

可以参考并复制模板：

```text
docs/templates/project-understanding-template.md
```

### 4. 填写文档内容

文档需要说明你对以下内容的理解：

- 项目目标；
- 整体链路；
- MVP 范围；
- 你当前最确定的理解；
- 你仍然存在的疑问。

不要求面面俱到，鼓励写出自己的真实理解和真实问题。

### 5. 提交 Commit

Commit 信息格式：

```text
docs: add project understanding by 你的姓名
```

示例：

```bash
git add docs/members/project-understanding-zhangsan.md
git commit -m "docs: add project understanding by zhangsan"
```

### 6. 推送分支并发起 Pull Request

```bash
git push origin learn/zhangsan
```

Pull Request 目标分支选择 `main`。

PR 标题格式：

```text
[学习作业1] 项目理解文档 - 你的姓名
```

### 7. 根据 Review 修改

收到管理者或组员的 Review 意见后，在原分支继续修改并提交即可。

示例：

```bash
git add docs/members/project-understanding-zhangsan.md
git commit -m "docs: update project understanding by zhangsan"
git push origin learn/zhangsan
```

## 完成参考

作业完成时应至少包含：

- 一份 `project-understanding-你的姓名.md`；
- 一次符合格式的 Commit；
- 一次格式规范的 Pull Request；
- 至少一轮 Review 交互。

## 管理者检查清单

Review 时可以检查：

- 分支名是否符合 `learn/你的姓名或昵称`；
- 文件是否位于 `docs/members/`；
- 文件名是否符合 `project-understanding-你的姓名.md`；
- Commit 信息是否符合要求；
- PR 标题是否符合要求；
- 文档是否覆盖项目目标、整体链路、MVP 范围和个人疑问；
- 成员是否根据 Review 意见进行了回复或修改。

## 常见问题

如果你不熟悉 Git 分支操作，可以参考：[Git 官方文档 - 分支基础](https://git-scm.com/book/zh/v2/Git-%E5%88%86%E6%94%AF-%E5%88%86%E6%94%AF%E7%AE%80%E4%BB%8B)。

如果你不清楚如何发起 PR，请联系组长或在群内提问。
