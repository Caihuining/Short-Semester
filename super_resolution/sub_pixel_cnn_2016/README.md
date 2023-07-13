# Super Resolution
超分辨率机器学习模型锐化和放大输入图像，以细化细节并提高质量。
## 模型结构
超分辨率使用高效的亚像素卷积层，用于提高网络任务中的空间分辨率。通过增加像素数，可以在不丢失输入图像的内容和特征的情况下对图像进行澄清、锐化和放大。
## 数据集
在 BSD300 数据集上使用 200 张训练图像中的裁剪进行训练。


## 训练及推理
### 环境配置
提供[光源](https://www.sourcefind.cn/#/service-details)拉取的训练以及推理的docker镜像：
* 训练镜像：jupyterlab-tensorflow:2.7.0-centos7.6-dtk-22.10-py37-latest
* 推理镜像：jupyterlab-tensorflow:2.7.0-centos7.6-dtk-22.10-py37-latest


#### 依赖
anaconda

### 预训练模型
model文件夹提供的预训练模型介绍，例如：

    Project
    ├── model
    └── └── super-resolution-10.onnx.onnx #对应的onnx模型

### 推理
推理引擎版本：
* onnx: 1.9.0 
* onnxruntime: 1.8.0


## 性能和准确率数据
	
				
| 模型 | 下载 | 下载 （附示例测试数据） | ONNX 版本 | Opset 版本 |
| :------: | :------: | :------: | :------: |:------: |
| Super_Resolution | 240 KB | 7.6兆字节 | 1.5.0 | 10  |

## 源码仓库及问题反馈
* https://github.com/Caihuining/Short-Semester/tree/main/super_resolution/sub_pixel_cnn_2016
## 参考
* https://github.com/onnx/models
