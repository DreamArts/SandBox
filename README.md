SandBox
=======

練習用リポジトリ

### GitHub運用ルール

 * GitHub-Flow

  https://gist.github.com/Gab-km/3705015

  * masterブランチと、開発(フィーチャー)ブランチで、管理する。
  * masterブランチは【プルリクエストに対するマージのみ】とする。
  * 開発者数人にコードレビュー(OKなら:+1:を記載)してもらったら、自分以外の誰かにマージしてもらう。

 * 追加ルール

  * 1機能毎に、1開発(フィーチャー)ブランチとする。
  * 開発(フィーチャー)ブランチの名前には、feature/ の接頭詞をつける。
  * 開発(フィーチャー)ブランチを作ったら、すぐに、masterブランチにプルリクエストする。(議論の履歴を残すため)


### 準備
```
$ git config --global push.default simple
```
```
$ git clone git@github.com:DreamArts/SandBox.git
$ cd SandBox
```

### 開発(フィーチャー)ブランチでの作業

ブランチ作成
```
$ git checkout -b feature/hoge_hoge
```

ブランチ登録
```
$ git push -u origin feature/hoge_hoge
```

編集 → add → commit → push
```
$ vi README.md

$ git add README.md
$ git commit
$ git push
```

masterブランチの内容を取り込みたい場合
```
$ git pull origin master
```

開発(フィーチャー)ブランチの内容を取り込みたい場合
```
$ git pull
```


### プルリクエスト
```
PULL REQUEST HERE
```

### マージしてもらった後の、後始末

masterに戻る
```
$ git checkout master
$ git pull
```

リモートで削除されたブランチの同期
```
$ git fetch --prune
```

不要になったローカルブランチの削除
```
$ git branch -d feature/hoge_hoge
```

### メンテナンス
不要になったリモートブランチの削除
```
$ git push origin :feature/hoge_hoge
```

リモートに存在するブランチを全て取得
```
$ git fetch --all
```

リモートブランチに存在しないブランチを削除する
```
$ git fetch --prune
```

## License
MIT Licence. Go WiLD!

## Contributor
