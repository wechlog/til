# 使い方
WechlogメンバーによるTIL(Today I learned)。
GitHubのリポジトリを使ってアウトプットを習慣化していきましょう◎

## 目的
共同開発で必須であるGitを使い慣れる。
TILを通じて共同開発のハードルを少しでも下げられたら嬉しいです。

## その他のメリット
各々、GitHubの草を残せます。
Gitの理解が深まります。

## 使い方
このリポジトリをForkしてローカルにgit clone。

```
git clone https://github.com/~~ご自身のアカウント~~/til.git
```

ローカル上でプロジェクト下に自身の名前でディレクトリを作成。あとは.mdでファイルを作成して好きに記述。

できたらプッシュ。

```
git remote rm origin
git init
git add .
git commit -m"changed title"
git remote add origin https://github.com/wechlog/til.git
git push -u origin master
```

GitHub上でプルリクエストする。

僕がマージして反映させます。