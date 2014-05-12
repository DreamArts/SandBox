SandBox
=======

練習用リポジトリ

```
$ git clone git@github.com:DreamArts/SandBox.git
$ cd SandBox
```

```
$ git checkout -b work
$ git push origin work

$ vi README.md
$ git add README.md
$ git commit
```

```
PULL REQUEST HERE
```

不要になったローカルブランチ・リモートブランチの削除
```
$ git branch -d hoge
$ git push origin :hoge
```

リモートに存在するブランチを全て取得
```
$ git fetch --all
```

リモートブランチに存在しないブランチを削除する
```
$ git fetch --prune
```

