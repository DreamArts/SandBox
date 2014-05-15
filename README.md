SandBox
=======

練習用リポジトリ

### GitHub運用ルール

 * GitHub-Flow

  https://gist.github.com/Gab-km/3705015

  * masterブランチは、プルリクエストに対するマージのみ、許可する。
  * 1機能 1開発(フィーチャー)ブランチ

 * 追加ルール

  * 開発(フィーチャー)ブランチの名前には、feature/ の接頭詞をつける。
  * 開発(フィーチャー)ブランチを作ったら、すぐに、masterブランチにプルリクエストする。(議論の履歴を残すため)
  * 自分以外の開発者にレビューしてもらい、:+1: をもらったら、自分以外の誰かがマージする。


### 準備
```
$ git clone git@github.com:DreamArts/SandBox.git
$ cd SandBox
```

### 作業用ブランチでの作業
```
$ git checkout -b work
$ git push origin work

$ vi README.md
$ git add README.md
$ git commit

$ git pull origin work
$ git push origin work
```

### プルリクエスト
```
PULL REQUEST HERE
```

### 後始末
不要になったローカルブランチの削除
```
$ git branch -d hoge
```

### メンテナンス
不要になったリモートブランチの削除
```
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

