# Coding Cheatsheets

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | **中文** | [日本語](README.ja.md) | [Русский](README.ru.md)

真正实用的开发者速查表

# # # 被实际使用的骗局

□ □ □ 吉特

{\fn方正准圆简体\fs12\1cHC9ECC4}什么?
|---|---|
`git log --oneline --graph --all` 视觉分支
`git stash && git stash pop` 公园+恢复工作 QQ
QQ `git reset --soft HEAD~1` 撤销上次承诺, 保留更改QQ
`git rebase -i HEAD~3` 重写最后 3 个承诺
`git bisect start` 二进制搜索错误 。
`git reflog` 逆行救生器
`git clean -fd` 删除未跟踪文件 QQ

# # # 贝壳 #

{\fn方正准圆简体\fs12\1cHC9ECC4}什么?
|---|---|
QQ `cmd1 && cmd2` 只有在 1 成功的情况下运行 2 。
`cmd | tee file` 打印和保存输出
`cmd > out 2>&1` 将 Stderr 重定向到 studout QQ
* `Ctrl-A / Ctrl-E` * * 开始/结束
QQ `!cmd` 重新运行上次匹配命令 QQ
`for f in *.log; do mv "$f" "$f.bak"; done` 打开文件

######## 卷曲(#######

{\fn方正准圆简体\fs12\1cHC9ECC4}什么?
|---|---|
~ `curl -s url | jq .` ~ 获取 + 剖析 JSON ~ ~
`curl -X POST -d '{"a":1}' -H 'Content-Type: json'` POST 身体 ===
`curl -o file url` 下载
`curl -v url` 调试请求
`curl --retry 5 url` 自动重试

*□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□单□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□□

{\fn方正准圆简体\fs12\1cHC9ECC4}什么?
|---|---|
`python3 -m http.server 8000` 即时文件服务器
`python3 -m json.tool < data.json` 漂亮的印刷 JSON ===
`[x*2 for x in range(10)]` 列表理解
`dict(zip(keys, vals))` 调用命令

{\fn华文楷体\fs16\1cHE0E0E0}安全快速

{\fn方正准圆简体\fs12\1cHC9ECC4}什么?
|---|---|
`ss -tulpn` 是什么在听吗?
`openssl s_client -connect host:443` TLS 握手调试
`hashcat -m 0 hash rockyou.txt` 破碎的MD5
`john --wordlist=w.txt hash` 开膛手约翰
`shasum -a 256 file` 校对:

□ □ 点球手

{\fn方正准圆简体\fs12\1cHC9ECC4}什么?
|---|---|
`docker ps -a` 所有容器
`docker exec -it c bash` 内壳
`docker logs -f c` 跟踪日志
`docker system prune -af` 核清理
~ `docker stats` ~ 现场资源使用量 ~
`docker run --rm -it img` 电离层容器

{\fn黑体\fs22\bord1\shad0\3aHBE\4aH00\fscx67\fscy66\2cHFFFFFF\3cH808080}# # # # # # # # Git 高级 #

{\fn方正准圆简体\fs12\1cHC9ECC4}什么?
|---|---|
`git worktree add ../wt branch` 第二次检票,同样的回购
`git cherry-pick abc123` 接受一个承诺
* `git branch -m old new` 重命名 *
`git diff main...feature` 3点=自差分起
`git commit --fixup abc && git rebase -i --autosquash` 干净的历史修补
`git push --force-with-lease` 安全力量推

□□□□□□□□□□

{\fn方正准圆简体\fs12\1cHC9ECC4}什么?
|---|---|
`rg -t py "import pandas"` 类型过滤搜索
`rg -l "TODO" | wc -l` 使用 TODOS 计数文件
QQ `rg "fn\w+" -A3` 匹配后的背景
`rg --files-without-match "test"` 文件缺少一些东西

□・・・・・・・雷格克斯

QQ 模式 QQ 匹配 QQ
|---|---|
@ @ `(?<=@)\w+` @ @ @ @ @ @ @ (看在后面) @ @
`\w+@\w+\.\w+` 邮件
`(\d{1,3}\.){3}\d{1,3}` IPv4 地址 QQ
`(?=.*[A-Z])(?=.*\d).{8,}` 密码验证器

□□□□□□□□□□□□□□□□□□□□

{\fn方正准圆简体\fs12\1cHC9ECC4}什么?
|---|---|
`.tables` 列表列表列表
`.schema tbl`表格 DDL
`.mode column` 可读输出 QQ
`.dump` 全部导出

---
## 贡献

欢迎提交 Pull Request，我们会审查并合并。由 [aixisstudio](https://github.com/aixisstudio) 维护，他也是开源应用防火墙 [Snitch](https://github.com/aixisstudio/Snitch) 的作者。

## 许可证: MIT
