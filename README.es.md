# Coding Cheatsheets

[English](README.md) | [Français](README.fr.md) | **Español** | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Cheat sheets de desarrollador que sí se usan

_El contenido detallado (listas, enlaces, descripciones) está en inglés por mantenibilidad — las secciones siguientes te guían._

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

---
## Contribuir

Los pull requests son bienvenidos: abre una PR y será revisada y fusionada. Mantenido por [aixisstudio](https://github.com/aixisstudio), autor de [Snitch](https://github.com/aixisstudio/Snitch), firewall de aplicaciones open source.

## Licencia: MIT
