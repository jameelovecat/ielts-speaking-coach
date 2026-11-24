# IELTS Speaking Coach · 雅思口语陪练

**先把自己的话说出来，再一起把它说得更好。**

这是一套面向 AI Agent 的雅思口语训练 Skill，重点适配 WorkBuddy 和 ChatGPT Skills。它把模考、专项训练、自由表达和复习分开，让练习有目标、有反馈，也留有自己的表达空间。

## 适合谁

- 想练雅思口语，但不想一开口就被打断纠错。
- 习惯先自己组织语言，再看修改建议和参考方向。
- 想把完整模考、刻意训练和日常自由表达分开进行。
- 希望从真实练习中积累常见问题、词汇搭配和表达结构。

本 Skill 只负责口语练习，不提供真题资料、录音工具或自动计时器。雅思口语评分和考试时长参考官方说明；AI反馈用于学习，不等同正式成绩。

## 设计方式

### 先说，再反馈

回答过程中不打断、不纠错、不提前给范文。说完后再按「原话 → 建议表达 → 简短原因 → 可选重试」给少量反馈，尽量保留你的意思、语气和个人风格。参考答案是练习后的可选方向，不是要背的标准答案。

### 模考和专项训练分开

完整模考按 Part 1、Part 2、Part 3 的考试流程进行，中途不教学，结束后再复盘；专项训练只练一个 Part 或一种能力，做完一题就聚焦一个改进点。另有三分钟自由口语日记和表达复习。

### 计划来自真实时间和练习记录

首次使用或模考后，Agent 会和你讨论目标、基础、每周时间和训练安排。提醒、文件记录和周报取决于平台当前功能与授权；没有真实记录时，不会编造时长、分数或进度。

## 安装与开始

### 最快方式：把仓库链接发给技能创建器

告诉 WorkBuddy 或 ChatGPT 的技能创建对话，使用这个公开仓库中的口语 Skill：

```text
https://github.com/jameelovecat/ielts-speaking-coach
```

并指定目录 `skills/ielts-speaking-coach/`。可以直接复制这句：

> 请根据这个 GitHub 仓库里的 `skills/ielts-speaking-coach/` 创建并安装雅思口语陪练 Skill，并读取该目录中的 references。

### WorkBuddy

打开「专家 · 技能 · 连接器」→「技能」→「添加技能」→「创建技能」，把上面的仓库链接和指令发给创建对话。创建后，说「开始练雅思口语」。

### ChatGPT

在 ChatGPT「Skills」中选择「Create」→「Create with chat」，发送上面的仓库链接和指令，按提示安装。Skills 是否可用取决于账号、工作区设置和产品开放范围；若看不到 Skills 入口，当前账号可能还不能安装。

### 命令行

使用支持 Skills CLI 的 Agent（例如 Codex）时，可直接运行：

```bash
npx skills add jameelovecat/ielts-speaking-coach --skill ielts-speaking-coach -g -a codex
```

如果创建对话无法读取 GitHub 仓库，仍可改用[WorkBuddy 安装包](dist/ielts-speaking-coach-workbuddy.zip)或[ChatGPT Skills 安装包](dist/ielts-speaking-coach-chatgpt.zip)上传。

### 豆包备用方式

普通豆包暂不提供完整 Skill 包。可以打开[豆包个人智能体备用设定](skills/ielts-speaking-coach/adapters/doubao-personal-agent.md)，复制其中的设定到智能体里使用。这个简版不承诺本地记录、自动提醒或周报。

## 练习入口

安装后直接选一句开始：

- 「带我做一轮 Part 1 专项训练，先让我自己回答。」
- 「开始一次完整口语模考，结束后再统一反馈。」
- 「我想自由说三分钟，聊聊今天发生的事。」
- 「复习表达本里的到期内容，一次考我一个。」
- 「先和我聊聊每周能练几次，再一起定一个计划。」

第一次练习前，Agent 会简单说明本次目标和大致用时；如要设置提醒，会先和你商量时间。真实作答时长需要语音或可靠计时功能支持。

## 留下反馈，一起迭代

这套练习方式来自真实使用，也需要更多人的实际反馈。练过之后，欢迎告诉我哪种引导有效、哪里卡住、你希望增加什么。

**Jamee／加米 · 加米实验室**

[GitHub @jameelovecat](https://github.com/jameelovecat) · [提交问题或建议](https://github.com/jameelovecat/ielts-speaking-coach/issues) · [X @Jamee_now](https://x.com/Jamee_now)

公众号「Jam Studio 加米实验室」欢迎扫码关注并留言：

<img src="assets/wechat-account-qr.png" width="220" alt="Jam Studio 加米实验室公众号二维码">

## 口语题库来源

练习可使用社区整理的 [zeeklog／IELTS 资料库](https://zeeklog.github.io/IELTS/)（[GitHub 仓库](https://github.com/zeeklog/IELTS)）。开始模考前，告诉 Agent 你要练的剑桥册数、Test 和 Part；Agent 应标出题目来源。仓库提供练习流程和来源指引，不打包第三方剑桥真题 PDF 或音频。

## 资料与隐私

- 本项目不打包剑桥真题 PDF、音频或个人练习答案；口语题目可通过上方社区资料库或你有权使用的资料练习。
- 不要把个人成绩、练习记录、录音或受版权保护的资料提交到公开仓库。
- Agent 能否读取文件、保留练习记录或创建定时提醒，取决于所用平台及你授予的权限。

## 来源

- [IELTS Speaking 考试结构](https://www.ielts.org/take-a-test/test-types/ielts-academic-test/ielts-academic-format-speaking)
- [IELTS Speaking 四项评分说明](https://ielts.org/news-and-insights/demystifying-the-ielts-speaking-test)
- [IELTS Speaking Band Descriptors](https://ielts.org/cdn/ielts-guides/ielts-speaking-band-descriptors.pdf)

使用规则见 [Skill 主文件](skills/ielts-speaking-coach/SKILL.md)，安装细节见[安装指南](docs/install.md)。欢迎通过上述渠道反馈，后续会根据实际使用情况持续改进。
