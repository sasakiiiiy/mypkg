# mypkg
* ロボットシステム学講義用のリポジトリである
* このリポジトリはROS2のパッケージである
* このリポジトリにはtalker.py,listener.py,talk_listen.launch.pyが含まれている

![test](https://github.com/sasakiiiiy/mypkg/actions/workflows/test.yml/badge.svg)
## 必要なソフトウェア
* ROS2
## 機能
* talker.py

パブリッシャを持つノードであり、0から数字をカウントしてトピック(countup)を通じてlistener.pyに送信する
* listener.py

サブスクライバを持つノードであり、トピック(countup)を通じてtalker.pyでカウントした数字を標準出力で出力する
## ダウンロード方法
gitコマンドを用いてローカル環境にmypkgリポジトリをクローンする
```bash
$ git clone https://github.com/sasakiiiiy/mypkg.git
```
## 実行例1
1. 端末を二つ開く
2. 実行コマンドを入力する

端末1
```bash
$ ros2 run mypkg talker
```

端末2
```bash
$ ros2 run mypkg listener　
```

3. 実行(端末2に出力される)

[INFO] [1672229123.345788640] [listener]: Listen: 0

[INFO] [1672229123.798582293] [listener]: Listen: 1

[INFO] [1672229124.298567609] [listener]: Listen: 2

[INFO] [1672229124.797972776] [listener]: Listen: 3

[INFO] [1672229125.297727952] [listener]: Listen: 4

[INFO] [1672229125.797026237] [listener]: Listen: 5

[INFO] [1672229126.297816656] [listener]: Listen: 6

[INFO] [1672229126.797432847] [listener]: Listen: 7

[INFO] [1672229127.298248778] [listener]: Listen: 8

[INFO] [1672229127.797516712] [listener]: Listen: 9

[INFO] [1672229128.297434582] [listener]: Listen: 10

## 実行例2

* talk_listen.launch.py

talker.pyとlistener.pyを1つの実行コマンドで実行させることができるもの

1. 実行コマンドを入力する

```bash
 $ ros2 launch mypkg talk_listen.launch.py
```
2. 実行

[INFO] [launch]: All log files can be found below /home/sasaki/.ros/log/2022-12-23-15-14-59-245522-DESKTOP-2HHRNAC-7434

[INFO] [launch]: Default logging verbosity is set to INFO

[INFO] [talker-1]: process started with pid [7436]

[INFO] [listener-2]: process started with pid [7438]

[listener-2] [INFO] [1671776100.070155034] [listener]: Listen: 0

[listener-2] [INFO] [1671776100.558072350] [listener]: Listen: 1

[listener-2] [INFO] [1671776101.057836003] [listener]: Listen: 2

[listener-2] [INFO] [1671776101.557980899] [listener]: Listen: 3

[listener-2] [INFO] [1671776102.058238508] [listener]: Listen: 4

[listener-2] [INFO] [1671776102.558258793] [listener]: Listen: 5

[listener-2] [INFO] [1671776103.058326989] [listener]: Listen: 6

[listener-2] [INFO] [1671776103.558340710] [listener]: Listen: 7

[listener-2] [INFO] [1671776104.058083231] [listener]: Listen: 8

[listener-2] [INFO] [1671776104.558622909] [listener]: Listen: 9

[listener-2] [INFO] [1671776105.057983873] [listener]: Listen: 10
## 動作確認済み環境
* Ubuntu
  * 22.04
## その他
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
* ©　2022 Yuto Sasaki
