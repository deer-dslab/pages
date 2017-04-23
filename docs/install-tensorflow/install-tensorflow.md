class: center middle
# Install Tensorflow

---
class: center middle
# Precondition
macOS Sierra  
Python 3.4
pyenv  
Anaconda3  
TensorFlow 1.0.1
2017/04/07

---
# Instruction
公式のインストールマニュアル (https://www.tensorflow.org/install/install_mac) の Installing with Anaconda を読む

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
Python 3.4 を使う  
コマンド中の tensorflow はただの仮想環境の名前

```shell
$ conda create -n tensorflow python=3.6 anaconda
$ source activate tensorflow
```

### インストール
Mac CPU version  
TensorFlow 1.0.1 for Python 3系

```shell
$ pip install --ignore-installed --upgrade https://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-1.0.1-py3-none-any.whl
```

Windows CPU version

```shell
$ pip install --ignore-installed --upgrade https://storage.googleapis.com/tensorflow/windows/cpu/tensorflow-1.0.1-cp35-cp35m-win_amd64.whl 
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
# Install Tensorflow おわり
[Topへ](..)