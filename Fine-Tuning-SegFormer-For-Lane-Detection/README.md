# Fine-Tuning SegFormer for Improved Lane Detection

以下是在RTX3060上，以13分钟/Epoch训练了30个Epoch的测试效果：
![视频1](https://github.com/user-attachments/assets/18943bc0-1239-4794-8bfa-774ce9df7667)
<table>
  <tr>
    <td><video width="300" height="200" controls><source src="https://github.com/user-attachments/assets/18943bc0-1239-4794-8bfa-774ce9df7667" type="video/mp4">您的浏览器不支持 video 标签。</video></td>
    <td><video width="300" height="200" controls><source src="https://github.com/user-attachments/assets/42a703e2-0d12-4e7a-9f30-9cbdc2ebbcf2" type="video/mp4">您的浏览器不支持 video 标签。</video></td>
    <td><video width="300" height="200" controls><source src="https://github.com/user-attachments/assets/ea32a666-b8be-42f2-8bdd-13e8a47be15e" type="video/mp4">您的浏览器不支持 video 标签。</video></td>
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
