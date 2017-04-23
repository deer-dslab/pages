class: center middle
# Install Keras

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
公式のインストールマニュアル (https://keras.io/ja/#_2) を読む

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

### インストール
Keras 2.0.2 をインストール

```shell
$ pip install keras==2.0.2
```

---
### 確認

```shell
$ python
>>> import tensorflow as tf
>>> hello = tf.constant('Hello, TensorFlow!')
>>> sess = tf.Session()
>>> print(sess.run(hello))
```

以下のメッセージが表示されたら正常
```shell
Hello, TensorFlow!
```

---
class: center middle
# Install Keras おわり
[Topへ](..)