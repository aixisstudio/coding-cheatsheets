# Coding Cheatsheets

[English](README.md) | **Français** | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Des antisèches de dev qui servent vraiment

_Le contenu détaillé (listes, liens, descriptions) est en anglais pour rester maintenable — les sections ci-dessous te guident._

## 📋 Cheat sheets that actually get used

## 🌿 Git

| Command | What |
|---|---|
| `git log --oneline --graph --all` | Visualize branches |
| `git stash && git stash pop` | Park + restore work |
| `git reset --soft HEAD~1` | Undo last commit, keep changes |
| `git rebase -i HEAD~3` | Rewrite last 3 commits |
| `git bisect start` | Binary-search the bug commit |
| `git reflog` | The undo-undo lifesaver |
| `git clean -fd` | Remove untracked files |

## 🐚 Shell

| Command | What |
|---|---|
| `cmd1 && cmd2` | Run 2 only if 1 succeeds |
| `cmd | tee file` | Print AND save output |
| `cmd > out 2>&1` | Redirect stderr to stdout |
| `Ctrl-A / Ctrl-E` | Line start / end |
| `!cmd` | Re-run last matching command |
| `for f in *.log; do mv "$f" "$f.bak"; done` | Loop over files |

## 🌐 curl

| Command | What |
|---|---|
| `curl -s url | jq .` | Fetch + parse JSON |
| `curl -X POST -d '{"a":1}' -H 'Content-Type: json'` | POST body |
| `curl -o file url` | Download |
| `curl -v url` | Debug the request |
| `curl --retry 5 url` | Auto-retry |

## 🐍 Python one-liners

| Snippet | What |
|---|---|
| `python3 -m http.server 8000` | Instant file server |
| `python3 -m json.tool < data.json` | Pretty-print JSON |
| `[x*2 for x in range(10)]` | List comprehension |
| `dict(zip(keys, vals))` | Zip to dict |

## 🔐 Security quickies

| Command | What |
|---|---|
| `ss -tulpn` | What's listening |
| `openssl s_client -connect host:443` | TLS handshake debug |
| `hashcat -m 0 hash rockyou.txt` | Crack MD5 |
| `john --wordlist=w.txt hash` | John the Ripper |
| `shasum -a 256 file` | Checksum |

## 🐳 Docker

| Command | What |
|---|---|
| `docker ps -a` | All containers |
| `docker exec -it c bash` | Shell inside |
| `docker logs -f c` | Follow logs |
| `docker system prune -af` | Nuclear cleanup |
| `docker stats` | Live resource usage |
| `docker run --rm -it img` | Ephemeral container |

## 🧵 Git advanced

| Command | What |
|---|---|
| `git worktree add ../wt branch` | Second checkout, same repo |
| `git cherry-pick abc123` | Take one commit |
| `git branch -m old new` | Rename |
| `git diff main...feature` | Three-dot = since divergence |
| `git commit --fixup abc && git rebase -i --autosquash` | Clean history fix |
| `git push --force-with-lease` | Safer force push |

## 🔍 ripgrep superpowers

| Command | What |
|---|---|
| `rg -t py "import pandas"` | Type-filtered search |
| `rg -l "TODO" | wc -l` | Count files with TODOs |
| `rg "fn\w+" -A3` | Context after match |
| `rg --files-without-match "test"` | Files lacking something |

## 📊 Regex

| Pattern | Matches |
|---|---|
| `(?<=@)\w+` | After @ (lookbehind) |
| `\w+@\w+\.\w+` | Emails |
| `(\d{1,3}\.){3}\d{1,3}` | IPv4 addresses |
| `(?=.*[A-Z])(?=.*\d).{8,}` | Password validator |

## 🗄️ SQLite

| Command | What |
|---|---|
| `.tables` | List tables |
| `.schema tbl` | Table DDL |
| `.mode column` | Readable output |
| `.dump` | Export everything |

---
## Contribuer

Les pull requests sont les bienvenues : ouvre une PR, elle sera relue et fusionnée. Maintenu par [aixisstudio](https://github.com/aixisstudio), auteur de [Snitch](https://github.com/aixisstudio/Snitch), pare-feu applicatif open source.

## Licence: MIT
