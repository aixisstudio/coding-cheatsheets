# Coding Cheatsheets

[English](README.md) | [Français](README.fr.md) | **Español** | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Cheat sheets de desarrollador que sí se usan

## 📋 Sábanas que en realidad se usan

## 🌿 Git

← Mando Silencioso
|---|---|
Silencio `git log --oneline --graph --all`
Silencio `git stash && git stash pop` Silencioso Park + restaurar el trabajo
← `git reset --soft HEAD~1` ← Undo último compromiso, mantener los cambios
Silencio `git rebase -i HEAD~3` Silencio Reescribir el último 3 commits
Silencio `git bisect start`  Binary-search the bug commit
Silencio `git reflog`
Silencio `git clean -fd` ← Eliminar archivos no rastreados

## 🐚 Shell

← Mando Silencioso
|---|---|
Silencio `cmd1 && cmd2` Silencio Run 2 sólo si 1 tiene éxito
Silencio `cmd | tee file` Silencio Imprimir Y guardar la salida
Silencio `cmd > out 2>&1` Silencio Redirect stderr to stdout
Silencio `Ctrl-A / Ctrl-E`
Silencio `!cmd` Silencio Re-run último comando matching ←
Silencio `for f in *.log; do mv "$f" "$f.bak"; done` Silencioso sobre los archivos

## 🌐 curl

← Mando Silencioso
|---|---|
Silencio `curl -s url | jq .` Silencio Fetch + parse JSON
confidencialidad `curl -X POST -d '{"a":1}' -H 'Content-Type: json'`
Silencio `curl -o file url` Silencio Descargar Silencio
Silencio `curl -v url`
confidencialidad `curl --retry 5 url`

## 🐍 Python one-liners

Silencio Silencio Silencio
|---|---|
Silencio `python3 -m http.server 8000` Silencio servidor de archivos instantáneos
Silencio `python3 -m json.tool < data.json` Silencio Bonita impresión JSON
confidencialidad `[x*2 for x in range(10)]`
confidencialidad `dict(zip(keys, vals))`

## 🔐 Security quickies

← Mando Silencioso
|---|---|
Silencio `ss -tulpn`
Silencio `openssl s_client -connect host:443`
Silencio `hashcat -m 0 hash rockyou.txt`
Silencio `john --wordlist=w.txt hash`
confidencialidad `shasum -a 256 file`

## 🐳 Docker

← Mando Silencioso
|---|---|
TENIDO `docker ps -a` TENIDO Todos los contenedores
Silencio `docker exec -it c bash`
Silencio `docker logs -f c` Silencio Sigue los registros
Silencio para la limpieza nuclear
Silencio `docker stats`
Silencio `docker run --rm -it img`

## 🧵 Git advanced

← Mando Silencioso
|---|---|
← `git worktree add ../wt branch` TENIDO Segunda salida, mismo repo TEN
Silencio `git cherry-pick abc123`
confidencialidad `git branch -m old new`
Silencio `git diff main...feature`
Silencio `git commit --fixup abc && git rebase -i --autosquash` Silencio Historia limpia
Silencio `git push --force-with-lease` ← Fuerza más segura

## 🔍 ripgrep superpowers

← Mando Silencioso
|---|---|
Silencio `rg -t py "import pandas"`
Silencio `rg -l "TODO" | wc -l` Silencio Contar archivos con TODOs
Silencio `rg "fn\w+" -A3`
Silencio `rg --files-without-match "test"` Silencio Archivos que faltan algo ←

## 📊 Regex

confidencialidad Pattern Silencioso
|---|---|
Silencio `(?<=@)\w+` Silencio Después de @ (lookbehind)
confidencialidad `\w+@\w+\.\w+`
Silencio `(\d{1,3}\.){3}\d{1,3}` Silencio IPv4 direcciones Silencio
Silencio `(?=.*[A-Z])(?=.*\d).{8,}` Silencioso validador de contraseña

## 🗄י SQLite

← Mando Silencioso
|---|---|
Silencio `.tables`
Silencio `.schema tbl` Silencio
Silencio `.mode column`
Silencio `.dump`

---
## Contribuir

Los pull requests son bienvenidos: abre una PR y será revisada y fusionada. Mantenido por [aixisstudio](https://github.com/aixisstudio), autor de [Snitch](https://github.com/aixisstudio/Snitch), firewall de aplicaciones open source.

## Licencia: MIT
