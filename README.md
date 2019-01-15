# Tacotron_BiaobeiData
An implementation of Tacotron speech synthesis using Biaobei data.

基于https://github.com/begeekmyfriend/tacotron/tree/mandarin
## 数据
使用最新发布的标贝数据，在此下载：
http://www.data-baker.com/open_source.html

下载后直接解压到项目的根目录下。项目需要使用到的数据是Wave文件夹下的语音文件和ProsodyLabeling文件夹下的语音标注文本。为了方便使用，将标注文本直接复制到Wave文件夹下。

建议：安装TensorFlow-gpu
## 预处理
pip install requirements.txt

python3 preprocess.py --dataset biaobei

预处理完会自动生成一个training文件夹。
## 训练
python3 train.py --name biaobei
