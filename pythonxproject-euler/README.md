# Python×ProjectEuler

Python×ProjectEuler勉強会用

## 内容

### 概要
PythonでProjectEulerの問題をひたすら解いていきます！

### 日時
2020/04/25（土）

### 場所
Zoom

※リンクがわからない方は@telumoまで連絡ください。

### 対象
- 興味のある方であれば誰でも
- プログラミングでどんなことやっているのかとりあえず見てみたい方

### 進め方
- T.B.D

**参考**

- issue: [Python×ProjectEuler · Issue \#4 · dangobro/Saturday\-Night\-Favorites](https://github.com/dangobro/Saturday-Night-Favorites/issues/4)

- Project Euler: [About \- Project Euler](https://projecteuler.net/)

- Hskell: [Welcome to Python\.org](https://www.python.org/)

## 事前準備

### Project Euler

事前にサインアップをお願いします。

[Register \- Project Euler](https://projecteuler.net/register)から簡単にできます。

### 環境構築

勉強会では、Python3.8の環境でProject Eulerの問題を解いていきます。

環境を完璧に合わせる必要はありませんが、少なくともPython3系の実行環境をご準備ください。

[Python Online \| ブラウザでプログラミング・実行ができる「オンライン実行環境」\| paiza\.IO](https://paiza.io/ja/projects/new?language=python3)などを利用すればローカルでの環境構築を行わずにブラウザ上でPython3が実行できます。


#### ローカル環境構築

※ここから先はローカルでの環境を合わせたい方のみ実施してください。

##### anyenvの設定

*Macユーザー向け*
```sh
# anyenvのインストール
$ brew install anyenv
# 設定ファイルに書き込み
# bash以外の方は`.bash_profile`部分を適宜直して実行シテください。（例：`.zshrc`など）
$ echo 'eval "$(anyenv init -)"' >> ~/.bash_profile
# シェルの再起動
$ exec $SHELL -l
```

*Mac以外のユーザー向け*
```sh
# ソースをクローン
$ git clone https://github.com/anyenv/anyenv ~/.anyenv
# パスを通す
# bash以外の方は`.bash_profile`部分を適宜直して実行シテください。（例：`.zshrc`など）
$ echo 'export PATH="$HOME/.anyenv/bin:$PATH"' >> ~/.bash_profile
$ echo 'eval "$(anyenv init -)"' >> ~/.bash_profile
# シェルの再起動
$ exec $SHELL -l
```

##### pyenvのインストール

```sh
# pyenvのインストール
$ anyenv install pyenv
# シェルの再起動
$ exec $SHELL -l
```

##### Python3.8.2のインストール

```sh
# Pythonの利用可能なバージョンを確認したい場合
$ pyenv install -l
# Python3.8.2のインストール（少々時間がかかります）
$ pyenv install 3.8.2
# インストール済みのバージョンを確認
$ pyenv versions
# > * system (set by /Users/username/.anyenv/envs/pyenv/version)
# >   3.8.2
# ローカルなバージョンを3.8.2に設定する
$ pyenv local 3.8.2
# グローバルなバージョンを設定したい場合はこちら
$ pyenv global 3.8.2
```

##### 仮想環境の設定

```sh
# 仮想環境の構築
$ python -m venv myenv
# 仮想環境の実行
$ source myenv/bin/activate
# 仮想環境の終了
$ deactivate
```