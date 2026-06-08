# writing-subsection-skills

[English](README.md) | [中文](README.zh-CN.md)

Codex skills for rewriting and auditing scientific manuscript subsections.

## Included skills

- `nature-abstract-skills`: writes and rewrites Nature/Science-style abstracts, then audits the text against six-step storyline, word limit, hard data, stand-alone readability, and hype control.
- `nature-introduction-skills`: rewrites biomedical or life-science Introduction text in a Nature/Science style, then audits the text against broad appeal, authentic knowledge gap, promise-evidence fit, citation sincerity, and narrative momentum.
- `nature-results-skills`: rewrites biomedical or life-science Results text in a Nature/Science style, then audits the text against figure evidence, logic chain, rigor, clutter, and claim-data fit.
- `nature-methods-skills`: rewrites Methods sections for reproducibility, then audits the text against methodological fit, transparent data pipelines, controls, statistical rigor, material validation, and data/code availability.
- `nature-discussion-skills`: rewrites biomedical or life-science Discussion text in a Nature/Science style, then audits the text against over-claiming, intellectual honesty, limitations, repetition, and broad impact.

## Install locally

Copy the skill folders into your Codex skills directory:

```powershell
Copy-Item -Path .\nature-abstract-skills -Destination "$env:USERPROFILE\.codex\skills\nature-abstract-skills" -Recurse
Copy-Item -Path .\nature-introduction-skills -Destination "$env:USERPROFILE\.codex\skills\nature-introduction-skills" -Recurse
Copy-Item -Path .\nature-results-skills -Destination "$env:USERPROFILE\.codex\skills\nature-results-skills" -Recurse
Copy-Item -Path .\nature-methods-skills -Destination "$env:USERPROFILE\.codex\skills\nature-methods-skills" -Recurse
Copy-Item -Path .\nature-discussion-skills -Destination "$env:USERPROFILE\.codex\skills\nature-discussion-skills" -Recurse
```

Then restart or refresh Codex so the skill metadata is rediscovered.
