class: center middle
# Keras Tutorial

---
class: center middle
# Precondition
macOS Sierra  
Python 3.4
pyenv  
Anaconda3  
TensorFlow 1.0.1  
Keras 2.0.2  
2017/04/07

---
# Instruction
[Kerasによる畳み込みニューラルネットワークの実装](http://aidiary.hatenablog.com/entry/20161120/1479640534) のコードを動かす  
一部 Keras 2.0.2 では動かなかったため修正

### 前準備
pyenv を使用していれば Anaconda 環境に切り替える
```shell
$ pyenv versions
* system (set by /Users/you/.pyenv/version)
  anaconda3-4.3.0

$ pyenv global anaconda3-4.3.0
(anaconda3-4.3.0) $ 
```
---

### 仮想環境を作成
[Install Tensorflow](../install-tensorflow) で作成した仮想環境 tensorflow を activate

```shell
$ source activate tensorflow
```

### コードのダウンロード
このリポジトリを Clone する

```shell
$ git clone https://github.com/f2um2326/keras-example.git
```

### Spyder 起動

```shell
$ spyder keras-example/mnist/mnist.py
```

---
### Run script
Press F5


<img src=./score.png width=400px>

---
class: center middle
# Keras Tutorial おわり
[Topへ](..)