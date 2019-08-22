# satellite image detection for aquaculture

简介：本项目利用 TensorFlow 图像识别（Object Detection）模式检测卫星图像（Satellite Image）或瓦片图像（Tile Image）中水产养殖网箱信息，并输出信息。

## 内容

## 方法

### 配置环境

* 安装并配置 Python3（推荐使用 Anaconda）

*注：若安装 Python3 程序，需将 python 写到环境变量。*

* 下载 TensorFLow

参照：https://www.tensorflow.org/install/pip

参照：https://github.com/pythonlessons/TensorFlow-object-detection-tutorial

参照：https://www.youtube.com/watch?v=HX2yXajg8Ts

Numpy 不兼容错误修正参考：https://blog.csdn.net/weixin_42081389/article/details/98185411

* 下载深度学习模型并安装protos

https://github.com/tensorflow/models

https://github.com/protocolbuffers/protobuf/releases/tag/v3.4.0 (mac 不需要)

在 research 目录下设置 Python 环境变量：
~~~bash
export PYTHONPATH=$PYTHONPATH:`pwd`:`pwd`/slim
~~~

安装 homebrew

参照：https://medium.com/@viviennediegoencarnacion/how-to-setup-tensorflow-object-detection-on-mac-a0b72fbf470a

~~~bash
protoc object_detection/protos/*.proto --python_out=.
~~~

* 验证环境配置

参照：https://pylessons.com/Tensorflow-object-detection-installation/

object_detection_tutorial.py No output images，参照：

https://github.com/tensorflow/models/issues/6684

### 标记图像

* 下载并安装图像标记软件

 参照：https://github.com/tzutalin/labelImg

* 标记图像

* 生成 Record 文件

### 训练模型

* 配置模型

* 训练模型

* 监视过程

* 导出模型

### 识别图像

* 验证模型

* 未完待续
 
