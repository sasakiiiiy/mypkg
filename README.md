# mypkg
* ROS2を学習するためのリポジトリである
* このリポジトリはROS2のパッケージである
# talk_listen.launch.pyコマンドの概要
![test](https://github.com/sasakiiiiy/mypkg/actions/workflows/test.yml/badge.svg)
## talk_listen.launch.pyコマンドの説明
パブリッシャを持つノードのtalker.pyコマンドによって、数字をカウントしてトピックを通じて送信し、サブスクライバ-を持つノードのlistener.pyコマンドで受信して表示させるコマンド
## 必要なソフトウェア
* ROS2
* Python
## talk_listen.launch.pyコマンドの使用方法
1. Ubuntuを開く
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
6. 実行例

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
