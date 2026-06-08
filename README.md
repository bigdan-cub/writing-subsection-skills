# writing-subsection-skills

Codex skills for rewriting and auditing scientific manuscript Results subsections.

## Included skills

- `nature-results-skills`: rewrites biomedical or life-science Results text in a Nature/Science style, then audits the text against figure evidence, logic chain, rigor, clutter, and claim-data fit.

## Install locally

Copy the skill folder into your Codex skills directory:

```powershell
Copy-Item -Path .\nature-results-skills -Destination "$env:USERPROFILE\.codex\skills\nature-results-skills" -Recurse
```

Then restart or refresh Codex so the skill metadata is rediscovered.
