# Coding Cheatsheets

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | **Русский**

Шпаргалки для разработчиков, которыми реально пользуются

##   Читы, которые действительно используются

## it Git

Командир, что такое
|---|---|
| `git log --oneline --graph --all` | Визуальные ветви
| `git stash && git stash pop` | Парк + восстановительные работы
`git reset --soft HEAD~1` Отменить последнее обязательство, сохранить изменения
`git rebase -i HEAD~3` Переписать последние 3 обязательства
| `git bisect start` | Binary-search the bug commit |
↑ `git reflog` | The undo-undo lifesaver[править править код]
| `git clean -fd` | Удалить неотслеживаемые файлы |

##Шелл

Командир, что такое
|---|---|
| `cmd1 && cmd2` | Запуск 2 только в случае успеха 1 |
| `cmd | tee file` | Печать и сохранение вывода |
| `cmd > out 2>&1` | Перенаправить stderr на stdout |
| `Ctrl-A / Ctrl-E` | Начало/конец строки
| `!cmd` | Перезапуск последней соответствующей команды |
`for f in *.log; do mv "$f" "$f.bak"; done` - Loop over Files

##   завиток

Командир, что такое
|---|---|
| `curl -s url | jq .` | Fetch + parse JSON |
`curl -X POST -d '{"a":1}' -H 'Content-Type: json'` | POST body |
| `curl -o file url` | Скачать
`curl -v url` Отладка запроса
`curl --retry 5 url` - Автозапуск

## - Python one-liners

Обсуждение Snippet What
|---|---|
`python3 -m http.server 8000` - Мгновенный файловый сервер
`python3 -m json.tool < data.json` Pretty-print JSON
| `[x*2 for x in range(10)]` | Понимание списка |
| `dict(zip(keys, vals))` | Zip to dict |

##Безопасность быстро

Командир, что такое
|---|---|
`ss -tulpn` - Что слушать
| `openssl s_client -connect host:443` | Отладка рукопожатия TLS |
`hashcat -m 0 hash rockyou.txt` - Crack MD5
Оригинальное название: John the Ripper
`shasum -a 256 file` | Checksum |

##   Докер

Командир, что такое
|---|---|
`docker ps -a` Все контейнеры
`docker exec -it c bash` - оболочка внутри
| `docker logs -f c` | Следуйте за журналами |
`docker system prune -af` - Ядерная очистка
| `docker stats` | Использование живых ресурсов
| `docker run --rm -it img` | Эфемерный контейнер

##   Продвинутый

Командир, что такое
|---|---|
| `git worktree add ../wt branch` | Вторая проверка, тот же РЕПО |
`git cherry-pick abc123` - Take one commit
| `git branch -m old new` | Переименование
| `git diff main...feature` | Три точки = с момента расхождения |
`git commit --fixup abc && git rebase -i --autosquash` - Чистая история
`git push --force-with-lease` Безопасный толчок

##   суперспособности

Командир, что такое
|---|---|
| `rg -t py "import pandas"` | Отфильтрованный по типу поиск |
| `rg -l "TODO" | wc -l` | Счет файлов с TODO
`rg "fn\w+" -A3` - контекст после матча
`rg --files-without-match "test"` - файлы, в которых чего-то не хватает

##   Регекс

Обсуждение Pattern | Matches
|---|---|
| `(?<=@)\w+` | После @ (см. ниже)
`\w+@\w+\.\w+` - Электронная почта
| `(\d{1,3}\.){3}\d{1,3}` | IPv4 адреса
| `(?=.*[A-Z])(?=.*\d).{8,}` | Валидатор паролей

##  ️ SQLite

Командир, что такое
|---|---|
| `.tables` | Таблицы списков |
| `.schema tbl` | Таблица DDL
| `.mode column` | Readable output
`.dump` Экспортировать все

---
## Участие

Pull request'ы приветствуются — открой PR, он будет проверен и принят. Ведёт [aixisstudio](https://github.com/aixisstudio), автор [Snitch](https://github.com/aixisstudio/Snitch) — open-source application firewall.

## Лицензия: MIT
