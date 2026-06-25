# 协作说明

本文档用于帮助成员完成学习小组的基础 Git 协作流程。

## 分支规范

所有成员都应从最新的 `main` 分支创建个人分支：

```bash
git checkout main
git pull origin main
git checkout -b learn/你的姓名或昵称
```

分支命名示例：

```text
learn/zhangsan
learn/xiaoming
learn/alice
```

## 文件规范

本次作业的个人文档统一放在：

```text
docs/members/
```

文件命名格式：

```text
project-understanding-你的姓名.md
```

示例：

```text
docs/members/project-understanding-zhangsan.md
```

可以复制模板文件后再填写：

```text
docs/templates/project-understanding-template.md
```

## Commit 规范

本次作业的 Commit 信息格式为：

```text
docs: add project understanding by 你的姓名
```

示例：

```bash
git commit -m "docs: add project understanding by zhangsan"
```

## Pull Request 规范

Pull Request 的目标分支应选择 `main`。

PR 标题格式：

```text
[学习作业1] 项目理解文档 - 你的姓名
```

PR 内容建议写清楚：

- 新增了哪份个人学习记录；
- 自己目前最确定的理解是什么；
- 自己还想请大家 Review 或讨论的问题是什么。

## Review 交互

收到 Review 意见后，不需要关闭 PR。直接在原分支继续修改、提交并 push，GitHub 会自动更新同一个 PR。

推荐回复方式：

```text
已根据建议补充了 MVP 范围理解，请再帮忙看一下。
```

## 常见问题

如果不熟悉 Git 分支操作，可以参考：[Git 官方文档 - 分支基础](https://git-scm.com/book/zh/v2/Git-%E5%88%86%E6%94%AF-%E5%88%86%E6%94%AF%E7%AE%80%E4%BB%8B)。

如果不清楚如何发起 PR，请联系组长或在群内提问。
