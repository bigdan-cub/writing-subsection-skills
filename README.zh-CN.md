# writing-subsection-skills

[English](README.md) | [中文](README.zh-CN.md)

用于改写和审查科研论文各类写作小节的 Codex skills。

## 已包含的技能

- `nature-abstract-skills`：编写和改写 Nature/Science 风格的摘要，并根据六步叙事、词数限制、硬数据、独立可读性和夸大控制进行审查。
- `nature-introduction-skills`：改写生物医学或生命科学论文的 Introduction，并根据跨学科可读性、真实知识鸿沟、承诺与证据匹配、引用诚实性和叙事推进感进行审查。
- `nature-results-skills`：改写生物医学或生命科学论文的 Results，并根据图文证据、逻辑链、严谨性、主线杂音和声明-数据匹配进行审查。
- `nature-discussion-skills`：改写生物医学或生命科学论文的 Discussion，并根据过度解读、学术诚实、局限性、重复度和广泛影响力进行审查。

## 本地安装

将技能文件夹复制到你的 Codex skills 目录：

```powershell
Copy-Item -Path .\nature-abstract-skills -Destination "$env:USERPROFILE\.codex\skills\nature-abstract-skills" -Recurse
Copy-Item -Path .\nature-introduction-skills -Destination "$env:USERPROFILE\.codex\skills\nature-introduction-skills" -Recurse
Copy-Item -Path .\nature-results-skills -Destination "$env:USERPROFILE\.codex\skills\nature-results-skills" -Recurse
Copy-Item -Path .\nature-discussion-skills -Destination "$env:USERPROFILE\.codex\skills\nature-discussion-skills" -Recurse
```

然后重启或刷新 Codex，让技能元数据被重新发现。
