# project-euler

Haskell×ProjectEuler勉強会用

## 内容

### 概要
HaskellでProjectEulerの問題をひたすら解いていきます。

### 日時
2020/04/25（土曜日）

### 場所
Zoom

※リンクがわからない方は@telumoまで連絡ください。

### 対象
- 下記の環境構築ができる方なら誰でも。

### 進め方
- T.B.D

**参考**

- issue: [Haskell×ProjectEuler · Issue \#1 · dangobro/Saturday\-Night\-Favorites](https://github.com/dangobro/Saturday-Night-Favorites/issues/1)

- Project Euler: [About \- Project Euler](https://projecteuler.net/)

- Hskell: [Haskell Language](https://www.haskell.org/)

## 事前準備

### Project Euler

事前にサインアップをお願いします。

[Register \- Project Euler](https://projecteuler.net/register)から簡単にできます。

### 環境構築

プロジェクトのクローン
```sh
# クローン
git clone https://github.com/dangobro/Saturday-Night-Favorites.git

# プロジェクトのディレクトリに移動
cd Saturday-Night-Favorites/project-euler
```

stackのインストール

（まだstackをインストールしていない方）
```sh
curl -sSL https://get.haskellstack.org/ | sh

# or

wget -qO- https://get.haskellstack.org/ | sh
```

（stackを既にインストール済みの方）
```sh
stack upgrade
```

バージョンの確認
```sh
stack --version

# Version 2.1.3, Git revision 0fa51b9925decd937e4a993ad90cb686f88fa282 (7739 commits) x86_64 hpack-0.31.2
```

サンプルアプリのビルド
```sh
stack setup
stack build
```

サンプルアプリの実行
```sh
stack run

# 次にように出力されれば成功です。
# Stack has not been tested with GHC versions above 8.6, and using 8.8.3, this may fail
# Stack has not been tested with Cabal versions above 2.4, but version 3.0.1.0 was found, this may fail
# someFunc
```

stackの参考

- [stack build](https://docs.haskellstack.org/en/stable/README/)