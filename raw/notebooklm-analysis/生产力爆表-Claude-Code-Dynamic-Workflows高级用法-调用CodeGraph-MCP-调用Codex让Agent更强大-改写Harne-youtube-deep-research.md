# YouTube 深度研究补充：Claude Code 进阶教程：Dynamic Workflow 高级玩法，省 Token 又高效！

## 基本信息

- YouTube: https://www.youtube.com/watch?v=9agd8rkKTvw
- Job ID: e1552e60-7513-4e34-b3ab-c058d47a1f73
- Status: completed
- Detected language: en
- Model: vertex:gemini-3.1-pro-preview

## 摘要

本期视频深入讲解了 Claude Code 中 Dynamic Workflow 的高级用法与实战技巧。作者演示了如何通过特定关键词激活该功能，并通过分析开源项目 issues、自定义各阶段 AI 模型（Opus/Sonnet/Haiku）来优化 Token 消耗。此外，视频还重点展示了如何在动态工作流中集成 MCP（如 codegraph）以及调用外部工具（如 CodeX CLI）进行代码交叉审查，极大提升了代码分析与 Bug 排查的效率，展现了 Dynamic Workflow 的强大潜力。

## 关键要点

- Claude Code 激活 Dynamic Workflow 的新关键词及基础操作演示
- 通过先生成 Workflow Plan 并审查执行阶段，有效控制 Agent 派生以节省 Token
- 自定义工作流各阶段的 AI 模型（如混用 Haiku 和 Sonnet），实现成本与性能的平衡
- 在 Dynamic Workflow 中成功调用 MCP（如 codegraph）进行深度的代码导航与分析
- 结合 CodeX CLI 与不同大模型进行代码交叉验证 Review，精准发现潜在 Bug 并复用脚本

## Clip 建议

- {'start': '00:00:46', 'end': '00:02:21', 'reason': '介绍了最新版激活 Dynamic Workflow 的关键词，并演示了如何要求先展示 plan 以节省 token 的核心技巧。'}
- {'start': '00:03:52', 'end': '00:05:21', 'reason': '详细展示了如何让 AI 输出工作流的执行阶段、Agent 数量及模型配置，是控制成本的关键步骤。'}
- {'start': '00:05:21', 'end': '00:06:36', 'reason': '实战演示如何将昂贵的 Opus 模型替换为 Haiku 和 Sonnet 的组合，极具实用价值的省钱技巧。'}
- {'start': '00:06:36', 'end': '00:08:44', 'reason': '高阶玩法演示，展示了如何在动态工作流中接入 MCP 工具进行代码导航和 Bug 分析，拓展了 AI 的能力边界。'}
- {'start': '00:08:44', 'end': '00:10:33', 'reason': '硬核实战，演示了调用外部工具 CodeX CLI 与多个大模型同时进行代码审查，发现潜在 Bug 的全过程。'}
- {'start': '00:10:46', 'end': '00:11:47', 'reason': '展示了如何在 VS Code 中查看生成的 JS 脚本以便后续复用，总结了工具集成的强大潜力。'}

## 文件链接

- analysis_md: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript?format=md
- transcript_csv: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript?format=csv
- transcript_json: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript
- transcript_srt: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript?format=srt
- transcript_txt: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript?format=txt
- transcript_vtt: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript?format=vtt
- translated_json: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript?translated=1
- translated_srt: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript?format=srt&translated=1
- translated_txt: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript?format=txt&translated=1
- translated_vtt: https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/transcript?format=vtt&translated=1

## 分片状态

- chunk 0: done start=0 transcript=https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/chunk/0
- chunk 1: done start=300 transcript=https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/chunk/1
- chunk 2: done start=600 transcript=https://youtube-research-workflow.hb67egcim4.workers.dev/job/e1552e60-7513-4e34-b3ab-c058d47a1f73/chunk/2

## Worker Analysis Markdown

# 视频分析报告

> 模型：vertex:gemini-3.1-pro-preview  |  视频语言：en

## 摘要
本期视频深入讲解了 Claude Code 中 Dynamic Workflow 的高级用法与实战技巧。作者演示了如何通过特定关键词激活该功能，并通过分析开源项目 issues、自定义各阶段 AI 模型（Opus/Sonnet/Haiku）来优化 Token 消耗。此外，视频还重点展示了如何在动态工作流中集成 MCP（如 codegraph）以及调用外部工具（如 CodeX CLI）进行代码交叉审查，极大提升了代码分析与 Bug 排查的效率，展现了 Dynamic Workflow 的强大潜力。

## 关键要点
- Claude Code 激活 Dynamic Workflow 的新关键词及基础操作演示
- 通过先生成 Workflow Plan 并审查执行阶段，有效控制 Agent 派生以节省 Token
- 自定义工作流各阶段的 AI 模型（如混用 Haiku 和 Sonnet），实现成本与性能的平衡
- 在 Dynamic Workflow 中成功调用 MCP（如 codegraph）进行深度的代码导航与分析
- 结合 CodeX CLI 与不同大模型进行代码交叉验证 Review，精准发现潜在 Bug 并复用脚本

## 推荐标题
1. Claude Code 进阶教程：Dynamic Workflow 高级玩法，省 Token 又高效！
2. AI 程序员必看！如何在 Claude 动态工作流中调用 MCP 与 CodeX 查 Bug
3. 压榨 Claude 极限：Dynamic Workflow 结合多模型交叉 Review 代码实战

## 视频简介
想知道如何将 Claude Code 的 Dynamic Workflow 发挥到极致吗？本期视频为你带来保姆级的高级用法教程！我们将实战演示如何通过生成 Workflow Plan 审计 Agent 行为，巧妙搭配 Opus、Sonnet 和 Haiku 模型来大幅节省 Token 成本。更硬核的是，视频详细讲解了如何在动态工作流中接入 MCP（codegraph）进行代码导航，以及调用 CodeX CLI 进行多模型交叉代码审查，轻松揪出隐藏 Bug。无论你是 AI 开发者还是效率极客，这些实战技巧都不容错过！点赞破千解锁更多高级教程，快来抄作业吧！

## 标签
Claude Code, Dynamic Workflow, AI代码审查, MCP集成, 大模型应用, 编程效率工具

## 精彩片段建议
- **00:00:46 → 00:02:21**：介绍了最新版激活 Dynamic Workflow 的关键词，并演示了如何要求先展示 plan 以节省 token 的核心技巧。
- **00:03:52 → 00:05:21**：详细展示了如何让 AI 输出工作流的执行阶段、Agent 数量及模型配置，是控制成本的关键步骤。
- **00:05:21 → 00:06:36**：实战演示如何将昂贵的 Opus 模型替换为 Haiku 和 Sonnet 的组合，极具实用价值的省钱技巧。
- **00:06:36 → 00:08:44**：高阶玩法演示，展示了如何在动态工作流中接入 MCP 工具进行代码导航和 Bug 分析，拓展了 AI 的能力边界。
- **00:08:44 → 00:10:33**：硬核实战，演示了调用外部工具 CodeX CLI 与多个大模型同时进行代码审查，发现潜在 Bug 的全过程。
- **00:10:46 → 00:11:47**：展示了如何在 VS Code 中查看生成的 JS 脚本以便后续复用，总结了工具集成的强大潜力。

## 完整字幕（原始）
```
在前几期视频中 我为大家讲解并且演示了cloudcode新增的dynamic workflow的用法 从最开始大家对dynamic workflows的质疑 到后来anthropic官方正式宣布cloudcode dynamic workflow功能 大家才对这个功能有了认可 而且无数开发者都对dynamic workflows这个功能大加赞赏 而且这几天很多粉丝私信让我继续讲 讲cloudcode dynamic workflow的高级用法 因为dynamic workflows确实非常强大 所以本期视频继续为大家分享cloudcode dynamic workflows的高级技巧 还有使用经验 本期视频如果点赞破签的话 后续我会继续为大家分享更多关于cloudcode高级用法的视频 在最新版的cloudcode中 anthropic官方将之前的workflow关键词改成了outrocode 输入之后我们只要看到这个关键词出现了这种见面效果 就说明在cloudcode中已经激活了dynamic workflows功能 在后面就可以跟上我们的任务 目前我使用cloudcode版本号是v2.1.162 在之前的视频中我为大家讲解过dynamic workflows它的概念原理 还分享了如何用更省token的方式来使用dynamic workflows 以及如何附用dynamic workflows的js脚本 下面继续为大家分享dynamic workflows更多高级用法 好下面我们就可以用opencloud这个开源项目的仓库进行测试 因为opencloud它有非常多的bug 然后我们就可以测试一下dynamic workflow来分析这些issues 在cloudcode中我们先输入outrocode 在后面我们就可以跟上我们的任务 然后我们看一下我输入的这个提示词 要求只读分析这个项目最近50个openissues 先展示workflow plan不要立即执行 在这里是这个目标要求他找出10个top10高优先级的issues 然后我们就可以直接运行 相见的话我们只需要使用outrocode就可以来启用dynamic workflows 在这个任务提示词中我们要求他先展示workflow plan 不要立即执行相见的话我们就可以来审计他生成的这个plan 而不是让他直接执行 因为直接执行的话他可能会派生出非常多的subagents 从而比较浪费token好这里他输出了workflow plan 在这里还提到识别到这是已经验证过的模式 然后我们看一下他生成的这个workflow的流程图 第一步他会先获取仓库中的50个issues 当确认抓取成功之后他才会调用这个workflow 在workflow的这个pipeline这里包括issues然后分析还有验证 在分析阶段每个issue会派一个agent 这些agent的数量会小于等于50 在验证这里每个issue也会分配一个agent 在最后合成这里只需要一个agent 在下面这里他给出了这个workflow js脚本的完整代码 然后我们就可以对这个代码进行审查 如果我们感觉没有问题就可以让他来执行 在阶段这里我们就可以看到这三个阶段 包括分析验证还有合成报告 在这里是他给出的这几个优先级信号 包括崩溃数据流失作为最高优先级 在这里还提到为什么验证阶段不可省 在最后这里就给出了运行前需要锁定两个会改变结果的决策 包括高优先级怎么排序 在这里我们就可以按照他的提示直接选第一项 在分析深度方面我们也可以按照他的提示来选 这里我们就默认选择第一项 但我们感觉这些没有问题之后 我们就可以直接按提交 让他来运行刚才生成的这个工作流 在这里他就提示workflow已经启动 而且这里输出了这三个阶段 我们就可以看到他一共派生了几十个agents 同时并发九个agents 下面我们还可以让cloudcode在执行dynamic workflow脚本之前 展示更加详细的信息 在任务这里还是和刚才一样的任务 在下面这里我们要求他在运行之前 先展示workflow的执行阶段 每个阶段预计使用多少agents 会检查哪些文件或目录 每个阶段使用什么模型停止条件是什么 最终验收标准是什么 并告诉他在批准之前不要开始执行 然后我们直接运行 这样的话我们就可以看到更加详细的workflow的信息 这里他就提示他已经设计好了这个workflow 然后我们看一下我们要求他输出的这些内容 包括这里的执行阶段 还有agent的数量 还有模型 还有检查员 第一阶段就是拉取最近50个open issues的全两元数据 在第一阶段是不需要使用agent的 所以这里数量是0 然后第二阶段就是每个assus的分析 这里是agent的数量 然后模型是ops模型 然后第三阶段就是通过对抗分析 判断这些assus是否修复是否重复等等 在agent的数量这里也是50 在模型这里还是ops模型 然后第4阶段就是对 由于上面产出的这些数据进行整理 并且合成最终的报告 在agent的数量这里是1 模型这里是ops 然后这里还给出了第五阶段 然后这里给出了这些agent的数量的合计 他给出了并发上线大概是10到14个 相近的话 在每一阶段他都使用ops模型 因为这个模型非常昂贵 然后我们可以让他将第二阶段 第三阶段所用到的模型都改成更加便宜的模型 比如说我们直接用提示词让他修改 将第二阶段和第三阶段的模型改成sunit模型 或者hyku模型 然后直接运行 然后紧接着他就为我们生成了这些组合建议 第一个建议就是第二阶段和第三阶段都用sunit的模型 然后第二个建议就是用hyku来分析 用sunit来验证 也就是第二阶段用hyku 第三阶段用sunit模型 然后第三个选项就是两阶段都用hyku 在这里我们就选择第二项他给出的这个组合 也就是用hyku分析 用sunit验证 我们直接选中 cloudcode就非常智能的帮我们设计了这些选项 然后这里就输出了第二阶段使用hyku 第三阶段使用sunit 在这个表格中就是这几个阶段所用到的模型 然后我们就可以根据他的提示按这个跑 让他来启动这个workflow 我们直接运行 然后我们就可以看到在这个阶段他用的都是hyku模型 然后我们再切到下一个阶段 在这个阶段他用的就是sunit模型 相近的话 我们就可以指定他在每个阶段所用到的模型是什么 这样的话就可以更加节省我们的token 好 下面我们继续测试 这一次我们可以让他来调用mcp 比如说这一次让他调用codegraph这个项目 让他对一个开源项目的仓库进行分析 因为codegraph这个项目他是支持mcp的 所以我们就可以让cloudcode通过codegraph的mcp 在dynamicworkflows中使用codegraph 下面我们就可以看一下我出的这个任务 要求他使用dynamicworkflow分析仓库中潜在的bug 这里告诉他了总预算为200万token 要求使用codegraphmcp做代码导航 并且要求重点关注这些模块 可能存在的bug 输出格式是简洁的markdown报告 并且要求他在完整执行之前 先展示workflow plan 在这里我们就给他了一个开源项目的仓库链接 也就是这个为opencloud开发的记忆系统的这个仓库 然后我们就可以直接运行 先让cloudcode根据我们的任务 先生成workflow plan 在这个任务中 我们设置了这个token的预算 还明确了 让他调用codegraphmcp 好 这里cloudcode就输出了这个workflow plan 在这里就是需要检查的这些代码文件 然后这里给出了五个阶段 然后在这里他给出了这几个选项 在这里我们就可以选择第一项 然后他提示这个最终报告应该怎么办 然后我们这里就选择输出并且保存 然后就直接提交cloudcode就会启用这个workflow 这里这个workflow正在运行 然后我们就可以来具体看一下 这是第一阶段 然后我们可以进入一个agent进行查看 进入之后 我们就可以看到他这里调用了codegraphmcp 然后我们还可以查看其他的agent 可以看到这里他都调用了codegraphmcp 而且在这里我们还可以看到他们调用的工具的数量 相见的话 我们就实现了在dynamicworkflow中 让这些agent来调用mcp 就可以发挥出dynamicworkflow更强大的潜力 好 下面我们可以继续测试 我们甚至可以在dynamicworkflow中调用codexcri 执行代码审查任务 我们可以看一下我输入的这个任务 让他用dynamicworkflow对这个开源项目 也就是opencloud记忆插件 做止读交叉验证review 目标就是找潜在bug不修改代码 要求启动三个review 包括调用codexcri的review 第二个review就是使用ops模型进行独立审查的review 第三个就是使用sunet模型进行独立审查的review 要求就是codexcri只启动一次 单一review不可用 就标记不可用 不能假装在执行 只做文件和代码证据的问题 最后这里就是要求他输出的这些内容 然后我们直接运行 好 这里提示这个工作流正在运行 下面我们就可以查看一下 在第一阶段这里有三个agent 第一个是调用codex的 第二个是调用了ops模型 第三个是调用了sunet模型 然后我们就可以进入第一个进行查看 进入之后 在命令这里 他正在调用codex命令 对这个项目进行审查 他是通过sunet模型来调用的codexcri执行的审查任务 在这里我们还可以看到他们所消耗的token 这个ops模型与sunet模型 他们消耗的token已经搭 达到了100多k 然后这个调用codexcli的agent 他只消耗了20k token 这里还会显示他调用了三个工具 也就是刚才我们查看的 他调用的这三个工具 相见的话 我们就成功在dynamic workflow中 引入了codexcli也参与代码的review 从而不单单只依靠cloud系列模型对代码进行review 因为codex他对代码的review能力也是非常强的 很多cloud无法发现的潜在bug 用codex反而能发现 好 在这里他输出了这个交叉验证的review报告 在这里就是最终确认的这些bug 一共有5个bug 这里是对这些bug的详细描述 在最后这里他就给出了这些修复建议 像这样的话 我们就完成了在dynamic workflow中 调用codexcli 以及ops模型 还有三枚的模型 对我们的开源项目做了review 并且成功发现了这5个潜在的bug 当我们下次还需要使用这个工作流的时候 我们就可以继续附用刚才cloudcode来生成的这个workflow的这个脚本 然后我们还可以在vs code中看一下这个脚本是如何调用codex的 在这里我们就可以看到他创建了一个agent 用这个agent来调用codexcli 驱动这个agent的模型是sunet的模型 像这样的话 下次我们就可以直接在cloudcode中来附用这个脚本 对其他项目进行交叉验证的review 这是我们测试的在dynamic workflow中调用codexcli 而且我们还可以在dynamic workflow中调用更多工具 从而让cloudcode更加强大 好 本期视频就做到这里 欢迎大家点赞关注和转发 谢谢大家观看
```

## 翻译字幕（zh）
```
在前几期视频中 我为大家讲解并演示了cloudcode新增的动态工作流的用法 从最开始大家对动态工作流的质疑 到后来anthropic官方正式宣布cloudcode 动态工作流功能 大家才认可这个功能 而且无数开发者都对动态工作流这个功能大加赞赏 而且最近很多粉丝私信让我继续说 讲云代码动态工作流的高级用法 因为动态工作流确实非常强大 所以本期视频继续为大家分享云代码动态工作流的高级技巧 还有使用经验 本期视频如果点赞破签的话 後续我会继续为大家分享更多关于云代码高级用法的视频 在最新版本的云代码中 anthropic官方将之前的workflow关键词改成outrocode 输入后我们只看到这个关键词出现了这种见面效果 就说明在Cloudcode中已启用动态工作流功能 在后面可以跟上我们的任务 目前我使用云代码版本号是v2.1.162 在之前的视频中我为大家讲解过动态工作流其概念原理 还分享了如何使用更省代币的方式来使用动态工作流 以及如何附用动态工作流的js脚本 下面继续为大家分享动态工作流更多高级用法 好下面我们可以用opencloud这个开源项目的仓库进行测试 因为opencloud它有非常多的bug 然后我们可以测试一下动态工作流来分析这些问题 在云代码中我们先输入outrocode 在后面,我们可以遵循我们的任务 然后我们看看我输入的这个提示词 要求只读分析此项目最近50个开放 先展示工作流程计划不要立即执行 在这里是这个目标要求他找出10个Top10高优先级的问题 然后我们可以直接运行 相见的话我们只需要使用outrocode就可以来启用动态工作流 在这个任务提示词中,我们要求他先展示工作流程计划 不要立即执行相见的话,我们可以来审查他生成的这个计划。 而不是让他直接执行 因为直接执行的话,他可能会派生出非常多的子代理人 从而比较浪费token好这里他输出工作流程计划 在这里还提到识别到这是已经验证的模式 然后我们看看他生成的这个工作流的流程图 第一步他会先获取仓库中的50个问题 当确认抓取成功后,他才会调用这个工作流 在工作流程上的这个管道这里包括问题然后分析还有验证 在分析阶段每个问题会派一个代理人 这些代理的数量会小于等于50 在验证这里每个问题也会分配一个代理 在最后合成这里只需要一个代理 在下面他给出了这个工作流 js脚本的完整代码 然后我们可以对这个代码进行审查。 如果我们觉得没有问题,我们可以让他执行 在这个阶段,我们可以看到这三个阶段。 包括分析验证和合成报告 这是他给出的这些优先信号。 包括崩溃数据流失作为最高优先级 这里还提到为什么验证阶段不可省。 最后在这里就给出了运行前需要锁定两个会改变结果的决定。 包括高优先级如何排序 在这里我们可以根据他的提示直接选择第一项 在分析深度方面,我们也可以按照他的提示来选择 这里我们默认选择第一项 但我们觉得这些没有问题之后 我们可以直接提交 让他运行刚刚生成的这个工作流 在这里他就提示workflow已经启动 而且在这里输掉了这三个阶段 我们可以看到他一共派生几十个特工 同时发送九个代理人 下面我们还可以让cloudcode在执行动态工作流脚本之前 显示更多详细信息 在任务中还是和刚才一样的任务 下面我们要求他在运行前 首先展示工作流的执行阶段 每个阶段使用多少代理 查看哪些文件或目录 每个阶段使用什么模型停止条件是什么 最终认可标准是什么 并告诉他在批准之前不要开始执行 然后我们直接运行 这样,我们就可以看到更详细的工作流信息。 这里他就表示他已经设计好了这个工作流 然后我们看看我们要求他输出这些内容 包括执行阶段 代理人的数量 还有模型 还有检查员 第一阶段是收集最近50个开放问题的全两元数据。 第一阶段不需要使用代理 这里的数量为0 第二阶段是每个对象的分析。 这里是代理人的数量 然后模型是ops模型 第三阶段是通过对抗分析。 判断这些assus是否修复或重复等等 在代理的数量也在这里50 在模型这里还是ops模型 第四阶段是对的。 由于上述数据进行整理 并合成最终的报告 在代理的数量这里是1 模型这里是ops 然后这里还给出了第五阶段,然后这里给出了这些代理的总数。 他给出并发上线大概是10到14个 相近的话 在每一阶段他都使用ops模型 因为这个模型非常昂贵 然后我们可以让他把第二阶段 第三阶段所使用的模型都改为更便宜的模型。 例如,我们直接用提示词让他修改 将第二阶段和第三阶段的模型改成sunit模型 或者hyku模型 然后直接运行 接着,他为我们创造了这些组合建议。 第一个建议是第二阶段和第三阶段都用sunit的模型 然后第二个建议就是用hyku来分析 用sunit来验证 也就是第二阶段用hyku 第三阶段用sunit模型 然后第三个选项就是两阶段都用hyku 在这里我们就选择第二项他给出的这个组合 也就是用hyku分析 用sunit验证 我们直接选中 cloudcode就非常智能的帮我们设计了这些选项 然后在这里输出第二阶段使用hyku 第三阶段使用sunit 在这个表中就是这几个阶段所用的模型 然后我们可以根据他的提示按这个跑 让他来启动这个工作流 我们直接运行 然后我们可以看到在这个阶段他用的都是hyku模型 然后我们再切到下一个阶段 在这个阶段他用的就是sunit模型 相近的话 我们可以指定他每个阶段所使用的模型是什么 这样的话可以更节省我们的代币 好 下面我们继续测试 这一次我们可以让他来调用mcp 例如这一次让他调用codegraph这个项目 让他对一个开源项目的仓库进行分析 因为codegraph这个项目他是支持mcp的所以我们就可以让cloudcode通过codegraph的mcp 在动态工作流中使用codegraph 下面我们可以看一下我出的这个任务 要求他使用dynamicworkflow分析仓库中潜在的bug 这里告诉他了总预算为200万token 要求使用codegraphmcp做代码导航 并要求重点关注这些模块 可能存在的bug 输出格式是简洁的标记报告 并要求他在完整执行之前先展示工作流程计划 在这里,我们给了他一个开源项目的仓库链接,也就是这个为opencloud开发的记忆系统的仓库。 然后我们可以直接运行先让cloudcode根据我们的任务 先生成workflow plan 在这个任务中 我们设置了这个代币的预算 还明确了 让他调用codegraphmcp 好 这里cloudcode就输出这个工作流程计划 在这里就是需要检查的这些代码文件 然后在这里给出了五个阶段 然后在这里他给了这些几个选项 在这里我们可以选择第一项 然后他提示这个最终报告应该怎么办 然后我们在这里就选择输出并保存 然后直接提交cloudcode就会启用这个工作流 这里这个工作流正在运行 然后我们就可以来具体看一下 这是第一阶段 然后我们可以进入一个代理进行查看 进入后 我们就可以看到他这里调用了codegraphmcp 然后我们还可以查看其他代理 可以看到这里他都调用了codegraphmcp 而且在这里我们还可以看到他们调用的工具的数量 相见的话 我们就实现了在动态工作流中 让这些代理来调用mcp 可以发挥出动态工作流更强大的潜力 好 下面我们可以继续测试 我们甚至可以在动态工作流中调用codexcri 执行代码审查任务 我们可以看一下我输入的这个任务 让他用dynamicworkflow对这个开源项目 也就是opencloud记忆插件 做止读交叉验证review 目标就是找潜在bug不修改代码 要求启动三个review 包括调用codexcri的review 第二个review就是使用ops模型进行独立审查的review 第三个就是使用sunet模型进行独立审查的review 要求就是codexcri只启动一次 单一review不可用 就标记不可用 不能假装在执行 只做文件和代码证据问题 最后在这里就是要求他输出这些内容,然后我们直接运行 好 这里提示这个工作流正在运行 下面我们可以查看一下 在第一阶段这里有三个代理 第一个是调用代码的 第二个是调用了ops模型 第三个是调用了sunet模型 然后我们就可以进入第一个进行查看 进入之后 在命令这里 他正在调用codex命令 对这个项目进行审查 他是通过sunet模型来调用的codexcri执行的审查任务 在这里我们还可以看到他们消耗的代币 这个ops模型与sunet模型 他们消耗的代币已经搭 达到了100多k 然后这个调用codexcli的代理 他只消耗了20k代币 这里还会显示他调用了三个工具,也就是刚才我们查看的他调用的这三个工具。 相见的话 我们就成功在动态工作流中 引入了codexcli也参与代码的review 从而不单单只依靠cloud系列模型对代码进行审查 因为codex 他对代码的审查能力也非常强大 很多cloud无法发现的潜在错误 用codex反而能发现 好 在这里他输出这个交叉验证的评论报告 在这里就是最终确认的这些bug 一共有5个bug 这里是这些bug的详细描述 在最后这里他就给出了这些修复建议 像这样的话 我们就完成了在动态工作流中 调用codexcli 以及ops模型 还有三枚的模型 对我们的开源项目做了review 并且成功发现了这5个潜在的bug 当我们下次还需要使用这个工作流时 我们可以继续附用刚才cloudcode来生成的这个工作流的这个脚本 然后我们还可以在vs代码中看这个脚本是如何调用codex的 在这里我们可以看到他创建了一个agent 用这个agent来调用codexcli 驱动这个代理的模型是sunet的模型 像这样的话 下次我们就可以直接在cloudcode中来附用这个脚本 对其他项目进行交叉验证的审查 这是我们测试的在动态工作流中调用codexcli 此外,我们还可以在动态工作流中调用更多工具,从而使云代码更强大。 欢迎大家点赞关注和转发 谢谢大家观看
```
