# IELTS Speaking Coach · 雅思口语陪练

**先把自己的话说出来，再一起把它说得更好。**

这是一个面向 AI Agent 的雅思口语练习 Skill，适配 WorkBuddy 和 ChatGPT Skills。它把口语模考、Part 专项训练、自由表达、表达复习和每周复盘放在同一套流程里。

## 可以用它做什么

| 模块 | 怎么练 |
| --- | --- |
| 完整口语模考 | 按 Part 1、Part 2、Part 3 完成一整场；中途不提示、不纠错，结束后再按评分维度复盘。 |
| Part 专项训练 | 选择 Part 或具体能力，先自己组织并说完，再获得少量针对性反馈；参考示范放在尝试之后。 |
| 三分钟口语日记 | 自由聊今天的经历或自选话题，不按考试打分；表达结束后再整理反馈。 |
| 表达本与间隔复习 | 从真实练习中积累词汇搭配、常用句型和回答结构；到期后先回忆、再核对和更新掌握情况。 |
| 学习计划与提醒 | 结合目标、基础和每周可用时间，一起安排练习和复习；提醒时间由用户确认。 |
| 每周周报 | 汇总本周练习、反复出现的问题、表达复习进展，并列出下周一至三个优先目标。 |

## 练习原则

### 先表达，后纠错

练习过程中不打断。回答完成后，反馈会围绕「原话 → 建议表达 → 简短原因 → 可选重试」展开，优先处理最值得改的少数问题，并尽量保留个人意思和表达风格。参考答案是可选示范，不要求背诵。

### 模考和专项训练分开

模考模拟考试流程，结束后统一复盘；专项训练围绕一个 Part 或能力，答完一题就练一个改进点。自由口语日记则用于练习日常连续表达，不套考试评分。

## 表达复习怎么进行

每次练习后，可以把值得复用的搭配、句型和表达结构整理进表达本。复习时，Agent 先给含义相近的提示，让你自己回忆或造句，再反馈是否自然、准确。只有你实际作答后，才更新该条目的掌握状态和下次复习日期。

复习间隔沿用你已有的安排；如果还没有，可以一起采用例如 **1、2、4、7、15、30 天**的间隔。平台不能保存文件时，Agent 会给出可复制的表达记录，不会假装已经写入。

## 学习计划和每周周报

第一次使用时，Agent 会先了解你的目标、基础、可投入时间和练习偏好。没有近期口语成绩时，会建议先安排一次诊断模考，再依据实际表现调整计划。计划应适合你的时间，不预设所有人每天练习多久。

周报根据实际练习记录整理，包含：

- 本周计划和实际完成的练习；有可靠计时记录时才汇报分钟数。
- 完成的模考、专项训练和口语日记。
- 反复出现的语法、词汇和组织问题，并附真实练习例句。
- 表达复习结果，以及仍待复习的内容。
- 下周一至三个优先目标和建议安排。

如果平台能读取记录并支持定时任务，可以按约定时间生成周报或发送提醒；否则，Agent 会提醒你回到对话并提供记录，再据此整理。没有记录时不会编造数据，也不会把提醒当成练习完成。

## 开始使用

最简单的方式，是把公开仓库链接和下面这句话发给 WorkBuddy 或 ChatGPT 的 Skill 创建对话：

```text
https://github.com/jameelovecat/ielts-speaking-coach
```

> 请根据这个 GitHub 仓库里的 `skills/ielts-speaking-coach/` 创建并安装雅思口语陪练 Skill，并读取该目录中的 references。

- **WorkBuddy**：打开「专家 · 技能 · 连接器」→「技能」→「添加技能」→「创建技能」，发送仓库链接和上面的指令。
- **ChatGPT**：在「Skills」中选择「Create」→「Create with chat」，发送仓库链接和上面的指令。Skills 是否可用取决于账号及工作区设置。
- **命令行**：支持 Skills CLI 的 Agent（例如 Codex）可以运行：

```bash
npx skills add jameelovecat/ielts-speaking-coach --skill ielts-speaking-coach -g -a codex
```

如果创建对话无法读取仓库，可上传 [WorkBuddy 安装包](dist/ielts-speaking-coach-workbuddy.zip)或 [ChatGPT Skills 安装包](dist/ielts-speaking-coach-chatgpt.zip)。普通豆包可参考[个人智能体备用设定](skills/ielts-speaking-coach/adapters/doubao-personal-agent.md)；这个简版不包含文件记录和定时提醒承诺。

安装后，可以直接说：

- 「带我练 Part 1，先让我自己回答，最后再反馈。」
- 「开始一次完整口语模考，结束后统一复盘。」
- 「我想自由说三分钟，聊聊今天发生的事。」
- 「把今天练习里值得复习的搭配和句型整理进表达本。」
- 「先和我确定每周计划，并安排每周复习和周报。」

## 题目来源

练习可使用社区整理的 [zeeklog／IELTS 资料库](https://zeeklog.github.io/IELTS/)及其 [GitHub 仓库](https://github.com/zeeklog/IELTS)，也可使用你提供且有权使用的材料。开始练真题时，可以指定剑桥册数、Test 和 Part；Agent 应标明题目来源。原创题会标注为雅思风格练习，不称作真题或预测。

本仓库提供练习 Skill 和资料来源指引，不打包第三方剑桥真题全文、PDF 或音频。不要把个人成绩、练习记录、录音或无权公开的材料提交到公开仓库。

## 反馈与联系

欢迎在 [GitHub 提交问题或建议](https://github.com/jameelovecat/ielts-speaking-coach/issues)，或通过 [X @Jamee_now](https://x.com/Jamee_now) 和公众号留言。后续会根据实际使用反馈持续改进。

**Jamee／加米 · 加米实验室**

公众号「Jam Studio 加米实验室」：

<img src="assets/wechat-account-qr.png" width="220" alt="Jam Studio 加米实验室公众号二维码">

## 参考资料

- [IELTS Speaking 考试结构](https://www.ielts.org/take-a-test/test-types/ielts-academic-test/ielts-academic-format-speaking)
- [IELTS Speaking 四项评分说明](https://ielts.org/news-and-insights/demystifying-the-ielts-speaking-test)
- [IELTS Speaking Band Descriptors](https://ielts.org/cdn/ielts-guides/ielts-speaking-band-descriptors.pdf)

更多规则见 [Skill 主文件](skills/ielts-speaking-coach/SKILL.md)、[计划与周报说明](skills/ielts-speaking-coach/references/weekly-learning-cycle.md)和[安装指南](docs/install.md)。
