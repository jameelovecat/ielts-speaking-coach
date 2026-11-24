# 安装口语陪练

本版优先适配 WorkBuddy 和 ChatGPT Skills。安装时优先把公开仓库链接发给平台的技能创建对话，不必先下载文件。普通豆包提供可复制的备用智能体设定。

仓库链接：`https://github.com/jameelovecat/ielts-speaking-coach`

请始终指定 `skills/ielts-speaking-coach/`，避免创建旧的四科版本。可复制以下指令：

> 请根据这个 GitHub 仓库里的 `skills/ielts-speaking-coach/` 创建并安装雅思口语陪练 Skill，并读取该目录中的 references。

## WorkBuddy

1. 打开 WorkBuddy「专家 · 技能 · 连接器」→「技能」→「添加技能」→「创建技能」。
2. 把上面的仓库链接和指令发送给创建对话。
3. 创建后开始新对话，说「开始练雅思口语」。

如果 WorkBuddy 的菜单名称有变化，请在技能管理页面寻找上传或导入入口。读取练习文件、设置提醒时，只授予你希望使用的权限。

## ChatGPT

1. 在 ChatGPT「Skills」中选择「Create」→「Create with chat」。
2. 发送上面的仓库链接和指令，按提示创建并安装。
3. 安装后开始新对话，说「开始练雅思口语」。

Skills 的开放范围受账号、工作区设置和产品可用性影响。如果当前没有 Skills 入口，可先在支持 Skills 的 WorkBuddy 中使用；ChatGPT 官方说明见 [Skills in ChatGPT](https://help.openai.com/en/articles/20001066-skills-in-chatgpt)。

## 命令行

支持 Skills CLI 的 Agent（例如 Codex）可直接运行：

```bash
npx skills add jameelovecat/ielts-speaking-coach --skill ielts-speaking-coach -g -a codex
```

如果创建对话无法读取 GitHub 仓库，可下载对应[WorkBuddy 包](../dist/ielts-speaking-coach-workbuddy.zip)或[ChatGPT Skills 包](../dist/ielts-speaking-coach-chatgpt.zip)，再从上传入口导入。

## 普通豆包备用设定

本版暂不制作豆包工作台 Skill 包。打开[豆包个人智能体设定](../skills/ielts-speaking-coach/adapters/doubao-personal-agent.md)，复制「智能体设定」一节到个人智能体中，然后说「开始练口语」。

这是轻量备用方式，不承诺读取本地学习档案、自动保存练习记录、设置定时提醒或生成周报；语音功能以豆包当前版本为准。

## 更新与资料安全

- 安装新版本前，保留你自己的表达本、计划和练习记录。
- 本仓库不包含雅思真题、音频、个人成绩、练习答案或录音。
- 不要把受版权保护的材料和个人学习资料提交到公开仓库。

平台功能可能变化，遇到界面差异时以应用当前页面和官方说明为准。
