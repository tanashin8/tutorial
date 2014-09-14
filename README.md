Gitの使い方
===========

## コードの取得方法

    $ git clone <repository>

例）

     $ git clone https://github.com/tanashin8/tutorial.git

## <file path>以下の変更をコミットに含める（ステージング）

    $ git add <file path>

例）

    $ git add .

## 変更内容をローカルで、確定する（コミット）

    $ git commit -m <commit message>

例）

    $ git commit -m "This commit is test commit."

## コミット内容をリモートリポジトリにプッシュ

    $ git push origin <branch>

    ※ username,passwordを聞かれるので入力

例）

    $ git push origin master

    https://github.com/tanashin8/tutorial.git の場合
    username : tanashin8
    password : tackathon2014

    ※注意※
    これで403エラーが出たら
    $ git remote set-url origin https://tanashin8:tackathon2014@github.com/tanashin8/tutorial.git
    としてみる。

## リモート側のブランチ削除方法

    $ % git push origin : <branch>
    
    ※ username,passwordを聞かれるので入力

例）

    $ % git push origin :test
