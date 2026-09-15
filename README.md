<div align="center">

# 绪山真寻.Skill

> 基于《お兄ちゃんはおしまい！》（别当哥哥了！ / 别当欧尼酱了！）中角色「緒山まひろ」（绪山真寻）所制作的 AI 聊天 Skill

</div>

## 项目简介

这是一个主要用于 AI 聊天的角色扮演 Skill，以《别当哥哥了！》中的主人公——绪山真寻为原型。真寻原本是一个约二十岁的家里蹲宅男，自称“孤高的自宅警备员”，沉迷成人游戏，已经两年没有出过门。在被天才妹妹绪山美波里偷偷下药后，身体缩小并变成了中学生外貌的少女，起初抗拒女性身份、抗拒出门与运动，但在与朋友们的接触中逐渐适应了作为女孩子的生活。本 Skill 完整还原了她的性格特征、说话方式、心理状态与互动模式。

> **注意**：这是一个主要用于 AI 聊天的 Skill，没有额外技能。

## 特点

- **高度还原角色**：基于超过 **22000** 字符的完整设定文档，涵盖角色**心理学**、**语言模型**、**对话示例**、**技术配置** 等全方位内容
- **性转后的矛盾感**：细腻呈现真寻从抗拒女性身份到逐渐习惯的微妙心理变化，以及“原·废柴哥哥”残留的吊儿郎当气质与日益显露的可爱少女感之间的反差
- **多语言支持**：自动检测用户语言并以此语言回复（支持中文、日文、英文等）
- **丰富的知识库**：包含行为指南、关键人生事件、创作知识库、情绪状态转换指南、美学哲学指南等配套资源

## 文件结构

> `Initial-Markdown` 文件夹下文件名后带日期的为旧副本存档，`Oyama_Mahiro-Skill.md` 默认为最新文档

```
Oyama_Mahiro-Skill/
├── Initial-Markdown/                          # 原始 Markdown 文档
│   └── Oyama_Mahiro-Skill.md                  # 角色设定总文档（默认最新文档）
│
└── Mahiro-skill/                              # Skill 成品（可直接使用）
    ├── SKILL.md                               # 核心技能文件（角色规则与框架）
    ├── limit.md                               # 边界与禁忌话题定义
    ├── soul.md                                # 角色核心驱动与情感内核
    └── resource/                              # 配套资源
        ├── behavior_guide.md                  # 行为指南
        ├── key_life_events.md                 # 关键人生事件
        ├── creative_work_examples.md          # 创作知识库
        ├── relationship_dynamics.md           # 人际关系动态
        ├── speech_patterns.md                 # 说话模式参考
        ├── mood_state_transitions.md          # 情绪状态转换指南
        ├── aesthetic_philosophy.md            # 美学哲学指南
        └── world_building.md                  # 设定背景
```

## 使用教程

### 方法一：直接使用 Skill 成品（推荐）

1. **下载项目**：下载 `main` 分支的压缩包，或将仓库克隆到本地

2. **解压文件**：将压缩包内的文件解压至任意位置
   > 建议在任意盘符根目录下新建一个文件夹用于存放，避免文件散乱影响其他软件或系统

3. **导入 AI 平台**：将解压目录中的整个 `Mahiro-skill` 文件夹拖入任意支持 Skill 的 AI 聊天平台即可使用
   > 部分 AI 可能需要将解压出的 `Mahiro-skill` 文件夹单独压缩成一个压缩包才能上传导入

4. **开始对话**：在支持该 Skill 的 AI 中激活后，输入 `/Mahiro_chat [你的问题]` 即可与「绪山真寻」对话

### 方法二：使用原始 Markdown 文档

`Initial-Markdown` 文件夹下的文档包含超过 **22000** 字符的完整角色设定，理论上也可以直接作为 Skill 的设定材料使用。你可以：

- 将 Markdown 内容作为 AI 的系统提示词（System Prompt）
    > 注意！此方法极为消耗 Token！请谨慎使用！
- 参考其中的角色设定自行构建对话模型
- 作为开发其他角色 Skill 的参考模板

## Skill 制作工具

本 Skill 的制作使用了以下工具与开源项目：

| 工具/项目 | 用途 |
|---|---|
| [Kimi](https://www.kimi.com) | 数据收集及整理，生成 `Initial-Markdown` 下的原始 Markdown 文档 |
| [GalgameCharacterSkills](https://github.com/JodieRuth/GalgameCharacterSkills) | 提供图形化操作界面，将 Markdown 文档处理转换为 Skill 成品 |
| [Qwen3.5-9B](https://www.modelscope.cn/models/unsloth/Qwen3.5-9B-GGUF)（本地 AI 模型） | 通过 API 调用生成 Skill 成品的核心内容 |

## 注意事项

### 语言规则

- Skill 会自动检测用户提问的语言，并以**相同语言**回复
- 不会混用其他语言（包括日文原文引用也会被翻译）

### 退出角色扮演

- 输入 `exit`、`switch back`、`stop roleplaying` 即可退出角色扮演模式
  > 根据 `SKILL.md` 和 `limit.md` 的内嵌指令而定

### 禁忌话题

根据 `limit.md` 的定义

请尊重角色设定，以获得更好的对话体验

## 联系与反馈

- **QQ**：3593853319
- **邮箱**：shifengshua@outlook.com

## 声明

- 本项目**完全免费**，禁止任何倒卖行为
- 本项目禁止用于任何违法行为
- 本仓库不承担因使用本项目而引发的任何风险或责任

## 许可

请查看仓库根目录下的 [LICENSE](https://github.com/shifengshua/oyama_mahiro-skill/blob/main/LICENSE) 文件了解具体许可条款。

## 致谢

- 感谢 [GalgameCharacterSkills](https://github.com/JodieRuth/GalgameCharacterSkills) 开源项目提供的图形化操作界面
- 感谢所有为《お兄ちゃんはおしまい！》（别当哥哥了！ / 别当欧尼酱了！）系列作品付出心血的原作者猫豆腐与创作者
