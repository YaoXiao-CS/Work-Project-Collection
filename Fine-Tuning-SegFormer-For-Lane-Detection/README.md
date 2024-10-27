# Fine-Tuning SegFormer for Improved Lane Detection

以下是在RTX3060上，以13分钟/Epoch训练了30个Epoch的测试效果：
[如果视频未在线显示，请访问本项目的issues](https://github.com/YaoXiao-CS/Work-Project-Collection/issues/1)



https://github.com/user-attachments/assets/4c1dd9fc-d4e4-4a37-b4f1-5dadd6be74cd



<table>
 <tr>
    <td><video width="300" height="200" controls><source src="./Appendix_files/146841430-1-16.mp4" type="video/mp4">您的浏览器不支持 video 标签。</video></td>
    <td><video width="300" height="200" controls><source src="./Appendix_files/videoplayback.mp4" type="video/mp4">您的浏览器不支持 video 标签。</video></td>
    <td><video width="300" height="200" controls><source src="./Appendix_files/VCG.COM.mp4" type="video/mp4">您的浏览器不支持 video 标签。</video></td>
  </tr>
  <tr>
    <td><video width="300" height="200" controls><source src="./result_output/output_video.mp4" type="video/mp4">您的浏览器不支持 video 标签。</video></td>
    <td><video width="300" height="200" controls><source src="./result_output/output_video2.mp4" type="video/mp4">您的浏览器不支持 video 标签。</video></td>
    <td><video width="300" height="200" controls><source src="./result_output/output_video3.mp4" type="video/mp4">您的浏览器不支持 video 标签。</video></td>
  </tr>
</table>

#### 目录结构树

```shell
.Fine-Tuning-SegFormer-For-Lane-Detection
├── Appendix_files				# Videos used to test.
│   ├── 146841430-1-16.mp4
│   ├── VCG.COM.mp4
│   └── videoplayback.mp4
├── Fine-Tune-SegFormer.ipynb			# Model Training.
├── README.md
├── best_model.pth				# torch.save. Need to download from Baidu Netdisk.
├── inference.py				# Python script for inference.
├── requirements.txt
├── result_output				# Lane-Detection result.
│   ├── output_video.avi
│   ├── output_video2.avi
│   └── output_video3.avi
└── segformer-b2-finetuned-ade-512-512		# Download from Hugging Face.
    ├── README.md
    ├── config.json
    ├── gitattributes
    ├── preprocessor_config.json
    ├── pytorch_model.bin
    └── tf_model.h5
```

#### 数据下载链接

[代码中使用到的数据集在dropbox上的链接--deep_drive_10K.zip](https://www.dropbox.com/scl/fi/40onxgztkbtqxvsg2d6fk/deep_drive_10K.zip?rlkey=8h098tbe9dry81jidtte1d9j5&dl=1)， 在百度网盘链接[点击跳转](https://pan.baidu.com/s/1HEjsozLEk40HXg4_n-s4OQ?pwd=gp4y)或如下复制；

```shell
通过百度网盘分享的文件：微调segformer进行车道线检测
链接：https://pan.baidu.com/s/1HEjsozLEk40HXg4_n-s4OQ?pwd=gp4y
提取码：gp4y
```

#### 预训练的SegFormer

[Hagging Face官网链接，点击跳转](https://huggingface.co/nvidia/segformer-b2-finetuned-ade-512-512)， 在百度网盘链接[点击跳转](https://pan.baidu.com/s/1HEjsozLEk40HXg4_n-s4OQ?pwd=gp4y)或如下复制；

```shell
通过百度网盘分享的文件：微调segformer进行车道线检测
链接：https://pan.baidu.com/s/1HEjsozLEk40HXg4_n-s4OQ?pwd=gp4y
提取码：gp4y
```
