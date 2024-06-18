# 贡献指南

在参与社区贡献之前，请先阅读我们的 [行为守则](CODE_OF_CONDUCT.md)。如果你已经做好了所有的准备，那么恭喜你已经可以开始参与社区的开源贡献了！

## 准备工作

如果你是第一次参与开源贡献，请先阅读我们的 [致新兴的贡献者们](https://github.com/orgs/SWPUOpenSource/discussions/5) 文章，了解如何快速地参与开源贡献。

在开始之前，请确保你已经按照我们的《致新兴的贡献者们》中的步骤做好了准备，你需要有一个 GitHub 账号，并在你的计算机中正确安装和配置 Git 工具。如果你在使用 GitHub 的过程中遇到任何问题，请参考 [GitHub 帮助文档](https://help.github.com/) 来获得帮助，也可以前往我们的 [GitHub 讨论区](https://github.com/orgs/SWPUOpenSource/discussions) 寻求帮助。当然，在我们的 [QQ 群](https://qm.qq.com/q/k97AolpdtY) 中也有很多志同道合的朋友，你可以通过 QQ 群随时与我们取得联系。

## 选择一个目标项目

你可以从我们的社区中选择一个你感兴趣的项目（可供贡献的项目列表见 [这里](https://github.com/orgs/SWPUOpenSource/discussions/2)），或者自己申请发起一个新的项目。你也可以在 [新手任务列表](https://github.com/orgs/SWPUOpenSource/discussions/3) 中找到一些简单的入门任务，帮助你熟悉项目的开发流程，快速参与社区贡献。

如果你已经确定好了你的目标项目，你可以在该的项目中，找到一个你感兴趣的任务，或者自己发起一个新的任务。你可以在项目的 `README.md` 文件中找到项目的自述和开发文档，或者在项目的 `issues` 页面中找到已有的任务。

在你开始之前，请确保你已经阅读了项目的 `README.md` 文件和 `CONTRIBUTING.md` 文件（如果有的话），了解项目的开发流程和规范。如果你遇到了任何问题，请在项目的 `issues` 页面中提出你的疑问，或者在我们的 [QQ 群](https://qm.qq.com/q/k97AolpdtY) 中寻求帮助。

请确保你已经详细阅读了项目的 `CONTRIBUTING.md` 文件，以确保你能正确地提交你的贡献。不同的开源社区可能对开源贡献流程的要求有所不同，例如可能使用不同的开发工具、代码风格、测试规范等。

## 开始你的贡献

### 贡献规范

> [!TIP]
> 这里陈述的是在西南石油大学开源社区的泛用贡献规范，在少数情况下，项目负责人可能在项目中有更多的具体要求，你应当以项目的具体要求为准。如果你贡献的项目在我们的社区之外，你可能需要遵守该社区的贡献规范。如果项目（或外部社区）没有明确的贡献规范，你可以尽可能遵守我们的社区贡献规范。

### 命名约定

#### 分支命名

- 主分支：`main`
- 开发分支：`dev` 或 `develop`（部分项目可能未启用）
- 发布分支：`release/<版本号>`（部分项目可能未启用）
- 功能分支：`feature/<功能名>`
- 修复分支：`fix/<问题名>`
- 热修复分支：`hotfix/<问题名>`
- 文档分支：`docs/<文档名>`
- 杂项分支：`chore/<任务名>`

#### 提交信息

1. 标题

   格式：`<类型>(<作用>): <简要描述>`

   可选类型：

   - `feat`：新功能（feature）
   - `fix`：修复 bug
   - `docs`：文档（documentation）
   - `style`：格式（不影响代码运行的变动）
   - `refactor`：重构（即不是新增功能，也不是修改 bug 的代码变动）
   - `test`：增加测试
   - `chore`：构建过程或辅助工具的变动
   - `perf`：性能优化
   - `ci`：CI 配置文件或脚本的变动
   - `revert`：回滚某个更早的提交
   - `build`：构建相关的变动

2. 正文（可选的）：详细描述你的修改，包括原因、解决方案、测试用例等，每行不应超过 72 个字符。
3. 关闭的 issue（可选的）：如果你的 PR 解决了一个 issue，请在 PR 的描述中关闭该 issue。

> [!TIP]
> 样例：
>
> 分支命名样例：
>
> ```text
> feat/add-user-authentication
> fix/login-error
> release/1.2.0
> hotfix/urgent-security-fix
> docs/update-readme
> ```
>
> 这是一个完整的提交信息样例：
>
> ```text
> feat(auth): add user authentication
>
> - Implemented login and register pages
> - Integrated authentication API
> - Added unit tests for authentication module
>
> Resolves #123
> ```
>
> 尽管在大多数时候，你可以仅提交`feat(auth): add user authentication`而不必详细描述，但在一些情况下，你的确可能需要提供更多的细节。例如在需要在提交中关闭某个 issue 时，你需要将提交消息写为`feat(auth): add user authentication (Resolves #123)`。

在你完成了一个任务之后，请确保你提交了一个 `pull request`（PR），并描述清楚你的贡献。PR 应该包含你所做的修改，以及你为什么做这些修改。PR 应该遵循项目的开发规范，并且经过项目的维护者的审查。

### 贡献流程

#### 1. Fork 项目

首先，你需要 Fork 项目到你的 GitHub 账户下。Fork 是 GitHub 上的一个功能，它允许你复制一个项目到你的账户下，这样你就可以在自己的账户下进行开发。

1. 打开 GitHub 页面，找到你想参与的项目。
2. 点击右上角的 `Fork` 按钮，将项目复制到你的 GitHub 账户下。

#### 2. Clone 项目

克隆项目到本地电脑上。克隆是将一个远程仓库（比如 GitHub 上的项目）复制到本地电脑上。

1. 打开你的 GitHub 页面，找到你 Fork 的项目。
2. 点击 `Code` 按钮，复制项目的 HTTPS 地址。
3. 在你的本地电脑上打开命令行工具，切换到你想存放项目的目录。
4. 输入 `git clone <项目的 HTTPS 地址>` 命令，克隆项目到本地。

   ```bash
   git clone https://github.com/<你的 GitHub 用户名>/<项目名>.git
   ```

#### 3. 创建分支

> [!TIP]
> 你可以使用现代的编辑器 VSCode 替代古老的开发环境和编辑器，在 VSCode 中，你可以轻松的在现代的图形化界面中实现新增、切换分支、提交代码等操作。在 VSCode 中安装 Git 插件之后，你在 VSCode 中的 Git 操作与下面所提及的指令是**完全等效**的。

在你克隆项目到本地之后，你需要创建一个分支。分支是 Git 版本控制系统中重要的概念，它允许你在同一个项目中同时开发不同的功能或修复不同的 Bug。

1. 切换到项目目录。

   ```bash
   cd <项目名>
   ```

2. 创建一个新的分支。

   ```bash
   git checkout -b <分支名>
   ```

   例如：

   ```bash
   git checkout -b fix/login-error
   ```

#### 4. 开发

在你创建好分支之后，你就可以开始开发了。在你开发的过程中，你需要注意以下几点：

1. 遵循项目的开发规范。
2. 编写清晰的提交信息。
3. 编写测试用例。
4. 保持代码风格一致。
5. 保持提交记录整洁。

#### 5. 提交

在你完成开发之后，你需要提交你的修改。提交是将你开发的修改保存到本地仓库的过程。

> [!TIP]
> 你可以在开发过程中进行多次代码提交来让你的提交记录保持整洁，这也便于审计你贡献的开发者理解你的意图。

1. 确认你的修改。

   ```bash
   git status
   ```

   确认你的修改是否都已添加到暂存区。

2. 添加修改到暂存区。

   ```bash
   git add .
   ```

   如果你想添加单个文件，可以使用 `git add <文件名>` 命令。

3. 提交修改。

   ```bash
   git commit -m "<提交信息>"
   ```

   例如：

   ```bash
   git commit -m "feat(auth): add user authentication (Resolves #123)"
   ```

4. 推送修改到远程仓库。

   ```bash
   git push
   ```

   请注意如果你第一次推送，你需要使用 `-u` 参数指定本地分支和远程分支的关联。

   ```bash
   git push -u origin <分支名>
   ```

#### 6. 创建 PR

在你完成提交之后，你需要创建一个 `pull request`（PR）。PR 是向项目的维护者请求合并你的代码到项目的过程。

1. 打开你的 GitHub 页面，找到你 Fork 的项目。
2. 点击 `Pull requests` 按钮，打开 `Pull requests` 页面。
3. 点击 `New pull request` 按钮，打开 `Open a pull request` 页面。
4. 在 `Open a pull request` 页面，选择你想合并的分支，并填写 PR 的标题和描述。
5. 点击 `Create pull request` 按钮，创建 PR。

#### 7. 等待审查

在你创建 PR 之后，项目的维护者会对你的 PR 进行审查。审查可能包括以下内容：

1. 代码风格检查。
2. 单元测试。
3. 集成测试。
4. 性能测试。
5. 兼容性测试。
6. 文档检查。

项目的审查者在审查 PR 之后，可能会有一些建议或要求。如果审查者发现你的 PR 有问题，你可以在评论中进行反馈。如果审查者已经确认你的 PR 合适，就会在随后将你的 PR 合并到主分支。

#### 8. 向我们社区告知你的贡献

在你完成 PR 审查并合入主分支之后，你可以前往 [来自西南石油大学社区的贡献清单](https://github.com/orgs/SWPUOpenSource/discussions/4) 告知我们你的贡献，请在该讨论的评论中引用你的贡献内容。任何参与相关开源贡献的开发者都将成为我们协会的贡献者。

## 结语

**感谢你对开源社区做出的贡献！**
