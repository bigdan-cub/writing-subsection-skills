# writing-subsection-skills

Codex skills for rewriting and auditing scientific manuscript subsections.

## Included skills

- `nature-results-skills`: rewrites biomedical or life-science Results text in a Nature/Science style, then audits the text against figure evidence, logic chain, rigor, clutter, and claim-data fit.
- `nature-discussion-skills`: rewrites biomedical or life-science Discussion text in a Nature/Science style, then audits the text against over-claiming, intellectual honesty, limitations, repetition, and broad impact.

## Install locally

Copy the skill folders into your Codex skills directory:

```powershell
Copy-Item -Path .\nature-results-skills -Destination "$env:USERPROFILE\.codex\skills\nature-results-skills" -Recurse
Copy-Item -Path .\nature-discussion-skills -Destination "$env:USERPROFILE\.codex\skills\nature-discussion-skills" -Recurse
```

Then restart or refresh Codex so the skill metadata is rediscovered.
