# ROS2のパッケージであるmypkgにはtalker.pyとlistener.pyを一度に立ち上げるtalk_listen.launch.pyコマンドが含まれている
# talk_listen.launch.pyコマンドの概要
![test](https://github.com/sasakiiiiy/mypkg/actions/workflows/test.yml/badge.svg)
## talk_listen.launch.pyコマンドの説明
パブリッシャを持つノードのtalker.pyコマンドによって、16ビットの符号付き整数が型であるメッセージをカウントしてトピックを通じて送信し、サブスクライバを持つノードのlistener.pyコマンドで受信して表示させるコマンド
## 必要なソフトウェア
* ROS2
* Python
## talk_listen.launch.pyコマンドの使用方法
1. ubuntuを開く
2. ROS2をインストールする
3. gitコマンドを用いてローカル環境にmypkgリポジトリをクローンする
```bash
git clone https://github.com/sasakiiiiy/mypkg.git
```
4. ros2_wsディレクトリに移動する
```bash
cd ~/ros2_ws
```
5. 実行コマンドを入力する
```bash
ros2 launch mypkg talk_listen.launch.py
```
## 動作確認済み環境
* Ubuntu
  * 22.04
## その他
* このソフトウェアパッケージは、3条項BSDライセンスの下、再配布および使用が許可されます。
* ©　2022 Yuto Sasaki
