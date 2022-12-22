# mypkg
# talk_listen.launch.pyコマンド
![test](https://github.com/sasakiiiiy/mypkg/actions/workflows/test.yml/badge.svg)
## 何をするためのソフトか？
ノードを実行して、listenerが出力するべき行を探すコマンド。
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
