
---

### ### 2. `[Git Error] error: src refspec main does not match any`

```markdown
# [Git Error] error: src refspec main does not match any

## Date:
- 2025-05-01

## Description:
- Unable to push to GitHub, Git returned "src refspec main does not match any."

## Environment:
- Local Git Repo using PowerShell

## Tools Involved:
- GitHub, Git CLI, PowerShell

## Troubleshooting Steps Taken:
1. Tried `git push origin main`
2. Error occurred because no commits had been made, and no `main` branch existed locally.

## Resolution:
- Created an initial commit first:
  ```powershell
  git add .
  git commit -m "Initial commit"
  git branch -M main
  git push -u origin main

Lessons Learned:
Always commit before pushing and make sure the branch exists.

References:
https://stackoverflow.com/questions/32201356
