# Git Cheatsheet

## Configure Git User

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

---

## 1. `git commit -m "message"`

- Records changes to the repository with a message.
- The resulting commit provides a **short commit code**.

---

## 2. `git log`

- Shows the **full revision history**.
  - a. Displays the **full commit hash**.
  - b. Shows the current **HEAD position**.

---

## 3. `git log --oneline`

- a. Shows a **short commit hash** with a single-line commit message.
- b. Omits other commit metadata for readability.

---

## 4. `git reset --soft | --hard <commit-id>`

- a. `--soft`: Recommended – Keeps changes in working directory; shows them in `git status`.
- b. `--hard`: Discards changes – deletes files and resets to the specified commit.

---

## 5. `git revert <commit-id>`

- a. Reverts a **specific commit** even if it's in the middle of the history.
- b. Requires a commit message justifying the revert.

---

## 6. `git revert <commit-id> --no-commit`

- Allows you to **revert without immediately committing**, so you can make changes and commit manually.

---

## 7. GitHub Personal Access Token (e.g., `ghp_...`)

- Used for authentication instead of passwords when using HTTPS with GitHub.

---

## 8. `git remote -v`

Displays the configured remote URLs:

```bash
origin  https://github.com/ntharish13/gitdemo.git (fetch)
origin  https://github.com/ntharish13/gitdemo.git (push)
```

---

## 9. `git pull -r`

- Performs a **rebase** when pulling recent changes to keep history linear.

---

## 10. `git remote set-url origin <git-url>`

- a. Updates the **fetch and push** URLs.
- b. Works even if you're inside a different repository.

---

## 11. `git remote set-url --push origin <url>`

- Only updates the **push URL**, leaving the fetch URL unchanged.

---

## 12. `git push -u origin master`

- a. `-u` sets the upstream reference (links your local branch with the remote branch).
