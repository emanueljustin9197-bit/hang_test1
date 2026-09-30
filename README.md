# hang_test

`hang_test` 是一个简易开源 Codex Skill，用于把零散笔记或简短需求整理成清晰、可执行的任务清单。

> Codex Skill 的正式标识不支持下划线，因此目录名和调用名使用 `hang-test`；展示名仍为 `hang_test`。

## 使用方法

将 `hang-test` 文件夹放在 Codex 可发现的 Skills 目录中，然后在对话中显式调用：

```text
$hang-test 请把下面的需求整理成任务清单：下周五前完成登录页，接入邮箱登录，并补充错误提示。
```

也可以直接提出“把这些笔记整理成可执行清单”一类请求，由 Codex 自动匹配该 Skill。

## 输入和输出样例

输入：

```text
下周五前完成登录页，接入邮箱登录，并补充错误提示。负责人还没定。
```

输出：

```text
登录页交付清单

- [ ] 完成登录页界面
- [ ] 接入邮箱登录功能
- [ ] 补充登录失败等错误提示
- [ ] 在下周五前完成交付

待确认

- 负责人
```

## 项目结构

```text
.
├── LICENSE
├── README.md
└── hang-test/
    ├── SKILL.md
    └── agents/
        └── openai.yaml
```

## 许可证

本项目采用 MIT License，可自由使用、修改和分发。
