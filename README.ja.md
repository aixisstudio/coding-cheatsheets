# Coding Cheatsheets

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | **日本語** | [Русский](README.ru.md)

本当に使われる開発者チートシート

## 実際に使用したくなるチートシート

## 🌿  

| コマンド | 使い方 |
|---|---|
| `git log --oneline --graph --all` | ブランチの見える化 |
| `git stash && git stash pop` | パーク + 復元作業 |
| `git reset --soft HEAD~1` | 最終コミットを解禁 | 変更 |
| `git rebase -i HEAD~3` | 最終3コミットを書き換える |
| `git bisect start` | バイナリー検索 バグコミ |
| `git reflog` | 無人ライフセーバー |
| `git clean -fd` | 追跡されていないファイルを削除します |

## 🐚 シェル

| コマンド | 使い方 |
|---|---|
| `cmd1 && cmd2` | 1 が成功した場合のみ 2 を実行 |
| `cmd | tee file` | 印刷・保存 |
| `cmd > out 2>&1` | `cmd > out 2>&1` | スタッダをダイレクト |
| `Ctrl-A / Ctrl-E` | ラインスタート | 終了 |
| `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | `!cmd` | 最後のマッチングを再開 |
| `for f in *.log; do mv "$f" "$f.bak"; done` | ファイルのループ |

## バスケットカール

| コマンド | 使い方 |
|---|---|
| `curl -s url | jq .` | フェッチ+パーズ JSON |
| `curl -X POST -d '{"a":1}' -H 'Content-Type: json'` | POSTボディ |
| `curl -o file url` | ダウンロード |
| `curl -v url` | リクエストをデバッグ |
| `curl --retry 5 url` | オートリトリー |

## パイソンワンライナー

| スニペット | 何 |
|---|---|
| `python3 -m http.server 8000` | インスタントファイルサーバ |
| `python3 -m json.tool < data.json` | プリプリントJSON |
| `[x*2 for x in range(10)]` | リストアップ |
| `dict(zip(keys, vals))` | ジップ・トゥ・ディクト |

## 🔐 セキュリティ クイック

| コマンド | 使い方 |
|---|---|
| `ss -tulpn` | お客様の声 |
| `openssl s_client -connect host:443` | TLSハンドシェイクデバッグ |
| `hashcat -m 0 hash rockyou.txt` | 亀裂 MD5 |
| `john --wordlist=w.txt hash` | ジョン・リッパー |
| `shasum -a 256 file` | チェックサム |

## スタッフ

| コマンド | 使い方 |
|---|---|
| `docker ps -a` | すべての容器 |
| `docker exec -it c bash` | シェルインサイド |
| `docker logs -f c` | フォローログ |
| `docker system prune -af` | 核クリーンアップ |
| `docker stats` | ライブリソース利用 |
| `docker run --rm -it img` | エフェメラルド容器 |

## 🧵 Git 高度な

| コマンド | 使い方 |
|---|---|
| `git worktree add ../wt branch` | 二次チェックアウト |
| `git cherry-pick abc123` | 1 コミット |
| `git branch -m old new` | 名前 |
| `git diff main...feature` | 三点=卒業後 |
| `git commit --fixup abc && git rebase -i --autosquash` | クリーンな歴史の修正 |
| `git push --force-with-lease` | 安全力プッシュ |

# # # 既定の ripgrep スーパーパワー

| コマンド | 使い方 |
|---|---|
| `rg -t py "import pandas"` | タイプ フィルター検索 |
| `rg -l "TODO" | wc -l` | TODOファイル数 |
| `rg "fn\w+" -A3` | 試合後のコンテキスト |
| `rg --files-without-match "test"` | 何か欠けているファイル |

## 正規表現

| パターン | マッチ |
|---|---|
| `(?<=@)\w+` | アフター@(外観) |
| `\w+@\w+\.\w+` | メール |
| `(\d{1,3}\.){3}\d{1,3}` | IPv4アドレス |
| `(?=.*[A-Z])(?=.*\d).{8,}` | パスワードバリデータ |

## ️️ SQLite

| コマンド | 使い方 |
|---|---|
| `.tables` | リストテーブル |
| `.schema tbl` | テーブル DDL |
| `.mode column` | 読みやすい出力 |
| `.dump` | 全てをエクスポート |

---
## 貢献

プルリクエストを歓迎します。レビューしてマージします。[aixisstudio](https://github.com/aixisstudio) による管理 — オープンソースのアプリケーションファイアウォール [Snitch](https://github.com/aixisstudio/Snitch) の作者です。

## ライセンス: MIT
