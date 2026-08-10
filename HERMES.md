# Hermes-specific fork of mattpocock/skills

## Upstream sync

```bash
git checkout main
git pull upstream main
git checkout hermes-tweaks
git rebase main
git checkout main
git merge hermes-tweaks
```

Resolve conflicts (rare — only if upstream touched the same lines). `hermes-tweaks` carries the local-only tweaks (skill deletions, description caps) — always rebase it onto fresh main and merge it back in. Never delete the branch.
