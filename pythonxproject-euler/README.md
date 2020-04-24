# 「非エンジニアのためのオトナのプログラミング教室 vol1. 」
[ ProjectEulerをPythonで解いてみた！！]

## 内容
- 数学問題の奥深さとPythonの面白さを伝える
- ※なお、日常生活には何の役にも立たないと思います。m(__)m

## 背景
- 最近、遂にABC予想の証明が完了したってよ。
  - [査読8年、京大教授の「ABC予想」証明理論 ついに論文誌掲載へ \.\.\.www\.itmedia\.co\.jp › articles › 2004/03 › news155](https://www.itmedia.co.jp/news/articles/2004/03/news155.html)
- 数学の世界って面白い。
- 備考：
  - [これからは、英語より物理を学ぶ時代！｜日経BizGate](https://bizgate.nikkei.co.jp/article/DGXMZO2843303022032018000000?page=8)
  - [世界の著名テック企業のCEOたちが大学で選んだ専攻は \.\.\.www\.businessinsider\.jp › post\-33750](https://www.businessinsider.jp/post-33750)
- ジェネレーションZ以降の世代は確実にプログラミング的な技能を身に着けて社会に進出してきますよ、と。
  - [「プログラミング教育必修化」ご存じですか？ \- Ｚ会Asteria](https://www.zkai.co.jp/z-asteria/ms/programming/p1/)
- プログラミングの世界に少しでもかじってみたい。

## 日時
2020/04/25（土）

## 場所
Zoom

※リンクがわからない方は@telumoまで連絡ください。

## 対象
- 四則演算ができるひと
- Linux系のOSを動かすひと

**参考**

- issue: [Python×ProjectEuler · Issue \#4 · dangobro/Saturday\-Night\-Favorites](https://github.com/dangobro/Saturday-Night-Favorites/issues/4)

- Project Euler: [About \- Project Euler](https://projecteuler.net/)

- Python: [Welcome to Python\.org](https://www.python.org/)

- [abc Conjecture and New Mathematics \- Prof\. Fumiharu Kato, Oct 7, 2017 \(with English subtitles\) \- YouTube](https://www.youtube.com/watch?v=fNS7N04DLAQ)
- [トポロジーと圏論の夜明け 佐野 岳人 \| プログラマのための圏論勉強会 \- YouTube](https://www.youtube.com/watch?v=h_YJDTdHhU4)
- [6\-5\. 圏論とHaskellは仲良し \- 大森 健児 \- YouTube](https://www.youtube.com/watch?v=hbaNIIDPf24)

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
