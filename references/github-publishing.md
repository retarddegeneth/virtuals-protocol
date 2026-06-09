# GitHub Publishing Notes

Auth options for pushing Hermes skills from Termux/CLI:
- `gh auth login` device flow; afterwards `gh repo create` or push existing repo.
- HTTPS with `GITHUB_TOKEN`; export before push and unset after.
- SSH keys under `~/.ssh/` added as repo Deploy Keys.

Hard gotcha: the remote repo must exist on GitHub before `git push` will work. A `404` from the GitHub API or HTTPS push means create the repo first.

Creating a PR after pushing to `main`:
1. Create/switch to a feature branch: `git checkout -b vhermes/...`
2. Commit and push that branch: `git push -u origin <branch>`
3. Create the PR against base `main`: `gh pr create --head <branch> --base main --title "..." --body "..."`
