# ✨ Git Notes — Cleaner, Friendlier Cheatsheet

This is a cleaned, user-friendly version of the README with a compact layout, quick start, and a categorized cheat sheet.

If you'd like me to replace README.md with this improved version, tell me and I'll update the main README directly.

---

## Quick Start
Install Git and configure your identity:

```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Clone a repo:

```bash
git clone https://github.com/<username>/<repo>.git
cd <repo>
```

---

## Common Workflow
Create a branch, commit work, and open a PR:

```bash
git checkout -b feature/your-feature
git add .
git commit -m "Short message"
git fetch origin
git pull --rebase origin main
git push -u origin feature/your-feature
```

---

## Cheat Sheet (Short)
- Setup: `git init`, `git clone`
- Stage/Commit: `git add`, `git commit` 
- Push/Pull: `git push`, `git pull --rebase`
- Branch: `git checkout -b`, `git merge`, `git rebase`
- Undo: `git restore`, `git reset`, `git clean -f`

---

## Contributing
Fork, branch, commit, keep in sync with upstream, and open a PR.

---

Made with ❤️
