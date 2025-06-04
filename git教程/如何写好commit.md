
编写清晰且专业的 commit 信息对于有效的代码管理和团队协作至关重要。好的 commit 信息不仅能描述代码的修改内容，还能为其他开发者提供必要的上下文。以下是一些编写专业 commit 信息的最佳实践：

1. 遵循格式
使用一致的格式很重要。下面是一个常见的规范格式（比如 Conventional Commits）：
```
<TEXT>
<type>(<scope>): <subject>
<body>
<footer>
```

type: 提交类型，如 feat、fix、docs、style、refactor、test、chore等。
scope: 可选，描述影响的模块或部分（如 auth、ui、api等）。
subject: 提交的简短描述，一般不超过 72 个字符。
body: 可选，更详细的描述，解释做了什么和为什么，推荐使用多行格式。
footer: 可选，包含相关的任务编号、引用的 issue 等信息。
2. 示例
以下是一些良好的 commit 信息示例：
```
<TEXT>
feat(auth): add JWT authentication middleware
This change introduces JWT-based authentication for our API.
Users can now log in and receive a token that they will
use for authenticated requests.
Closes #42
<TEXT>
fix(ui): correct button alignment on mobile screens
Resolved an issue where buttons were not properly aligned
on mobile devices, improving overall user experience.
```
3. 清晰和简洁
简洁明了：提交信息应尽量简短明了，避免模糊不清的表述。
使用动词：采用命令式动词描述变更，例如“添加”、“修复”、“删除”等，使其更具指令性。
4. 提供上下文
解释：在 body 中，详细描述所做的更改、改变的原因以及可能的影响。
引用问题：如果相关，引用相关的 bug 单、问题单或任务编号，让其他开发者能够快速找到相关信息。
5. 使用语气
命令式：使用现在时的主动语态，而不是过去式。例如，“增加用户登录功能”比“增加了用户登录功能”更为合适。
6. 持续培训
团队一致性：通过会议或文档确保团队都遵循相同的 commit 风格，保持一致性。
7. 使用工具
linting 工具：考虑使用 commitlint 等工具来检查 commit 信息的格式。
模板：可以使用 commit message template 功能，预设 commit 信息格式，使得编写时更为高效。
遵循这些最佳实践，可以帮助你和你的团队维护更有条理、更专业的代码库，使得代码的历史变得更容易理解。
add new