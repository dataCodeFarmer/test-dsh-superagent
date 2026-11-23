# test-dsh-superagent

Test repository for dsh-superagent.

Use this repository to try requests from Feishu and review the pull requests created by the agent.

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
