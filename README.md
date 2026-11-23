# test-dsh-superagent

Test repository for dsh-superagent.

Use this repository to try requests from Feishu and review the pull requests created by the agent.

## 项目说明

本仓库用于测试 `dsh-superagent` 的协作流程：在飞书中提交任务，由代理修改仓库并创建拉取请求（Pull Request，简称 PR），最后由人工审核和合并。

仓库目前仅包含文档，没有需要安装或运行的应用。建议提交范围明确的小任务，便于检查结果；现有英文使用说明保留在下方。

## 使用流程

### 1. 准备工作

- 使用已配置 `dsh-superagent` 且关联本仓库的飞书群聊。
- 确保可以在 GitHub 上访问本仓库并查看 PR；合并操作需要相应的仓库权限。

### 2. 通过飞书提交任务

在群聊中提及 `@dsh-superagent`，说明目标文件、期望结果和限制条件，并要求创建 PR。例如：

```text
@dsh-superagent 请在 README.md 中增加一段中文项目简介，保留现有内容，完成后创建 PR 并把链接回复到这里。
```

不要要求将密码、访问令牌或私密聊天内容写入 GitHub。若代理在原对话中请求补充必要信息或访问权限，请在该对话中回复。

### 3. 查看结果与反馈

任务完成并可供审核后，在原飞书对话中打开代理回复的 PR 链接。阅读 PR 描述，在 **Files changed** 中逐项核对修改是否符合要求，并检查可用的自动化检查结果。

如需调整，在 PR 中留下审核意见。PR 已创建不代表已经审核通过或合并；可在 GitHub PR 页面查看当前状态。

### 4. 人工审核并合并 PR

由人工审核者确认修改符合预期、必要反馈已处理，并检查仓库要求的检查结果。确认可以合并后，由有权限的人员在 GitHub PR 页面执行合并；代理不会自动合并 PR。

合并后，确认 PR 状态为 **Merged**，并在目标分支查看最终内容。若没有合并权限，请联系有权限的仓库维护者处理。

## Usage

### Prerequisites

- Use a Feishu chat where `dsh-superagent` is configured to work with this repository.
- Make sure you can access this repository on GitHub to review the resulting pull request.

This repository contains only documentation; there is no application to install or run.

### Submit a request

1. In the configured Feishu chat, mention `@dsh-superagent` and describe the change you want.
2. Specify the target file, the expected result, and any constraints. Keep test requests small and focused.
3. Ask the agent to create a pull request so you can review the change before it is merged.

For example:

```text
@dsh-superagent Add a short section to README.md explaining the purpose of this test repository, and create a PR. Keep the existing content.
```

Do not include passwords, access tokens, or private chat content in changes intended for GitHub.

### Review the result

1. Open the pull request linked in the original Feishu conversation when the change is ready for review.
2. Read the PR description and inspect **Files changed** to confirm the result matches your request. Check any available automated checks as well.
3. Leave review comments on the PR if changes are needed. If the agent asks for missing information or access in Feishu, respond in that conversation.
4. A human reviewer decides whether to approve and merge the PR; the agent does not merge it automatically.
