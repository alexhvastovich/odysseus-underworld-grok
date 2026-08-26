# Publish to GitHub

The repo is committed locally on branch `main`. Use one of the options below.

## Option A — Cursor agent (recommended)

If prompted, add a **GitHub Personal Access Token** as `GH_TOKEN` with `repo` scope, then ask the agent:

> Push odysseus-underworld-grok to GitHub as a public repo

Create token: https://github.com/settings/tokens → Fine-grained or classic with **repo** access.

## Option B — GitHub CLI (local machine)

```bash
git clone <this-folder-or-copy> odysseus-underworld-grok
cd odysseus-underworld-grok
gh auth login
gh repo create odysseus-underworld-grok --public --source=. --remote=origin --push
```

## Option C — Manual

```bash
cd odysseus-underworld-grok
git remote add origin git@github.com:alexhvastovich/odysseus-underworld-grok.git
git push -u origin main
```

(Create the empty repo on GitHub first if it doesn't exist.)

## Expected repo URL

https://github.com/alexhvastovich/odysseus-underworld-grok
