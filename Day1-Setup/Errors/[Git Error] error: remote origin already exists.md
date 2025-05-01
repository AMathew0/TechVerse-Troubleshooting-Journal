
---

### ### 3. `[Git Error] error: remote origin already exists`

```markdown
# [Git Error] error: remote origin already exists

## Date:
- 2025-05-01

## Description:
- Tried to add a GitHub repo URL using `git remote add origin`, but got an error.

## Environment:
- Local Git Repo using PowerShell

## Tools Involved:
- Git, GitHub

## Troubleshooting Steps Taken:
1. Ran:
   ```powershell
   git remote add origin https://github.com/amathew0/TechVerse-Troubleshooting-Journal.git

Got error: remote origin already exists

Resolution:
Verified existing remotes:

powershell
Copy
Edit
git remote -v
If needed, changed the remote:

powershell
Copy
Edit
git remote set-url origin https://github.com/amathew0/TechVerse-Troubleshooting-Journal.git
Lessons Learned:
Use git remote -v to inspect existing remotes.

Only one remote called origin can exist at a time.

References:
https://git-scm.com/docs/git-remote
