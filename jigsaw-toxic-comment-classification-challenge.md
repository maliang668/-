#jigsaw-toxic-comment-classification-challenge

##说明
- 此项目在AWS执行，配置为：<br>
12 Core CPUs<br>
40G RAM <br>
100G SSD DISK<br>
Tesla K80<br>
-   操作系统及内核版本:<br>
Distributor ID:	Ubuntu<br>
Description:	Ubuntu 16.04.4 LTS<br>
Release:	    16.04<br>
<br>
-   开发软件环境如下:<br>
<br>
gensim              3.6.0 <br>
ipython             6.4.0 <br>
ipython-genutils    0.2.0 <br>
ipywidgets          7.3.0 <br>
jupyter-client      5.2.3 <br>
jupyter-core        4.4.0 <br>
Keras               2.2.0 <br>
Keras-Applications  1.0.2 <br>
Keras-Preprocessing 1.0.1 <br>
lightgbm            2.2.2 <br>
Markdown            2.6.11<br>
nltk                3.4   <br>
notebook            5.6.0 <br>
numpy               1.14.5<br>
pandas              0.22.0<br>
pip                 10.0.1<br>
scikit-learn        0.19.2<br>
scipy               1.1.0 <br>
seaborn             0.9.0 <br>
tensorboard         1.10.0<br>
tensorflow          1.9.0<br>
tensorflow-gpu      1.10.0<br>
xgboost             0.80<br>
<br>
##   运行时长
-   数据向量化大概五分钟，textcnn模型10分钟，bi-lstm模型90分钟，LR模型20分钟.<br>
-   使用Kfold训练，textcnn和bi-lstm均需要200分钟左右<br>
-   最后对CV预测进行拟合，10分钟左右.<br>

##   关支持材料
-   fasttext、glove的预训练词向量<br>
-   保存的最优模型和stacking导出的submission，按照代码均可得到