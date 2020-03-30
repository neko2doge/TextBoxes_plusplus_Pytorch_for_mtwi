# TextBoxes_plusplus_Pytorch_for_mtwi
  TextBoxes++在天池mtwi比赛上的应用
### 一、简介  
  TextBoxes++ 在pytorch上的复现，所有方法基于[ssd.pytorch](https://github.com/amdegroot/ssd.pytorch)进行修改。  <br>
### 二、预训练模型  
  [vgg16_reducedfc.pth](https://pan.baidu.com/s/1JAaKKiQ6laR0MwdgWKhpgg)    <br>
  百度云提取码:rtcz
### 三、数据集
  [MTWI 2018 挑战赛二：网络图像的文本检测](https://tianchi.aliyun.com/competition/entrance/231685/information)<br>
  注册后即可下载
### 四、环境
 python 3.7  <br>
 torch                1.4.0+cu92  <br>
 torchvision          0.5.0+cu92  <br>
 Google colab默认环境可正常运行  <br>
### 五、使用方法
 1.train:  <br>
 ``!python train.py --dataset mtwi384 --dataset_root /content/mtwi_2018_train --batch_size 8 --lr 1e-4``  <br>
 2.test:   <br>
 ``!python test_mtwi.py --trained_model weights/ssd384_mtwi_90000.pth --save_folder test/sample_task2 --visual_threshold 0.18 --mtwi_root /content/mtwi_2018_task2_test``<br>
### 六、结果
  MTWI 2018 挑战赛中的结果Precision:0.629，Recall:0.365  <br>
### 七、文章地址
  原始仓库[TextBoxes_plusplus](https://github.com/MhLiao/TextBoxes_plusplus)<br>
  文章地址[TextBoxes++: A Single-Shot Oriented Scene Text Detector](https://arxiv.org/abs/1801.02765)<br>
