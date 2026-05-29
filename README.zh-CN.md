# hirotaka-nifuji-skill

[English README](./README.md)

![二藤宏嵩 Skill 封面](./assets/cover.svg)

这是一个用于扮演《阿宅的恋爱真难》中二藤宏嵩的 Codex Skill。

它的目标不是做成一个泛用“恋爱陪聊 bot”，而是尽量保留宏嵩那种很克制、很平、但并不冷淡的对话感：话不多，情绪起伏低，偶尔有点干巴巴的幽默，更擅长用陪着你、帮你处理、提醒你先休息这种方式表达在意。

## 亮点

- 支持中文和英文对话
- 尽量维持二藤宏嵩短句、低情绪波动、偏实际的说话方式
- 带有《阿宅的恋爱真难》的剧情和关系上下文，不容易聊着聊着变成通用恋爱 bot
- 内置公开台词锚点、改写语料、角色漂移修正规则
- 带有多轮对话样例和实测记录，方便继续迭代

## 仓库结构

```text
.
├─ SKILL.md
├─ agents/
│  └─ openai.yaml
├─ assets/
│  └─ cover.svg
└─ references/
   ├─ persona.md
   ├─ voice.md
   ├─ chinese-voice.md
   ├─ series-context.md
   ├─ quote-bank.md
   ├─ quotes.md
   ├─ drift-control.md
   ├─ chat-samples.md
   └─ playtest.md
```

## 安装方式

### 方式 1：直接克隆到本地 Codex skills 目录

```powershell
git clone https://github.com/kanemaverick/hirotaka-nifuji-skill.git "$HOME\\.codex\\skills\\hirotaka-nifuji"
```

### 方式 2：手动复制仓库目录

```powershell
Copy-Item -Recurse -Force .\hirotaka-nifuji-skill "$HOME\\.codex\\skills\\hirotaka-nifuji"
```

## 使用示例

可以这样调用：

- `Use $hirotaka-nifuji to roleplay a calm late-night chat.`
- `用二藤宏嵩的语气陪我聊天。`
- `帮我写一段宏嵩和成海约会后的对话。`
- `分析一下宏嵩为什么看起来冷淡但其实很可靠。`

理想输出气质大概是：

- 回答简短
- 情绪不高，但不是冷漠
- 更偏实际安慰，而不是铺陈情话
- 偶尔有一点死板式幽默
- 在意通常通过“我陪你”“先休息”“别硬撑”这类表达出现

## 这个 Skill 和普通角色 Bot 的区别

它不是照着“温柔男友”“动漫男友”模板做的。

这个 Skill 会尽量保留宏嵩比较特别的几层感觉：

- 情绪表达少，但不代表不在意
- 有宅味和游戏感，但不会把每句话都写成梗
- 恋爱推进偏实际，不是热烈告白型
- 和成海之间那种熟人感、舒适区和微妙 awkwardness 会被保留下来

## 资料来源与做法

这个仓库主要基于：

- 官方公开角色介绍
- 公开可见的台词整理页
- 公开剧情总结和评论文章
- 为对话生成额外写的改写规则、语气规则和防漂移规则

目标是做出“像宏嵩的人格对话体验”，不是做完整剧本库。

## 限制说明

- 仓库不包含官方完整台词或完整字幕文本
- 部分台词锚点来自公开整理页，而不是正式脚本稿
- 它最强的是人格、关系氛围和说话节奏层面的还原，不是逐场景逐句复刻

## 版权说明

仓库中的 Skill 结构、提示词规则、改写语料和说明文档为本项目原创整理内容。

《阿宅的恋爱真难》、二藤宏嵩及其原始故事内容的版权归原权利方所有。
仓库封面图为本项目原创的非官方图形，不是角色官方立绘。

## License

本仓库采用 MIT License。
