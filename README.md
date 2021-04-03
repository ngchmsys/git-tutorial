# Git

## 開発の流れ

**クローンしてくる**

```sh
git clone https://backlog.com/repo
```

**ブランチを確認する(リモートも含める：-a)**

```sh
git branch -a
```

**ブランチを切る**

```sh
git branch Topic-branch-name
```

**ブランチを変更する**

```sh
git checkout Topic-branch-name
```

**ブランチを切って変更する**

```sh
git checkout -b Topic-branch-name
```

**ローカルリポジトリの状態を確認する**

```sh
git status
```

**ステージ領域に追加する(すべてのファイル)**

```sh
git add .
```

**コミットする**

```sh
git commit -m "コミットコメント"
```

**ブランチを削除する**

```sh
git branch -d ブランチ名
```

**コミットを取り消す**

```sh
git reset --hard ハッシュ値
```


# 初期設定

**ローカルリポジトリを初期化する**

```sh
git init
```

**コンフィグを設定する**

- system: Gitがインストールされたディレクトリ配下のgitconfig
  - C:\>where /R c:\ /T  gitconfig 
       365   2020/07/24      17:41:48  c:\Git\etc\gitconfig
- global: ログインユーザのHOMEディレクトリ配下の .gitconfig
- local: 対象リポジトリ内の .git/config

```sh
git config --global user.name "username"
git config --global user.email "username@example.com"
```

**コンフィグを確認する(リスト表示：-l)**

```sh
git config --list
```

**コンフィグを確認する（正規表現）**

```sh
git config --get-regexp ^user
```

**コンフィグを消去**

```sh
git config --global --unset user.name
```
