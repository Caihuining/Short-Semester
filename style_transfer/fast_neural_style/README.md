# Fast Neural Style Transfer
这种艺术风格转移模型将一个图像的内容与另一个图像的样式混合在一起。样式的示例可以在此 PyTorch 示例中看到。
## 模型结构
该模型使用实时样式传输和超分辨率以及实例规范化的感知损失中所述的方法。
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
    │   ├── candy-9.onnx
    │   ├── pointilism-9.onnx
    │   ├── rain-princess-9.onnx
    │   ├── udnie-9.onnx
    └── └── mosaic-9.onnx

### 推理
推理引擎版本：
* onnx: 1.9.0 
* onnxruntime: 1.8.0


## 性能和准确率数据
	
				
| 模型 | 下载 | 下载 （附示例测试数据） | ONNX 版本 | Opset 版本 |
| :------: | :------: | :------: | :------: |:------: |
| Mosaic |	6.6 MB |	7.2 MB |	1.4 |	9
| Candy	| 6.6 MB |	7.2 MB |	1.4 |	9 
| Rain Princess |	6.6 MB |	7.2 MB |	1.4	 |9
| Udnie	| 6.6 MB |	7.2 MB |	1.4 |	9
| Pointilism |	6.6 MB |	7.2 MB |	1.4 |	9

## 源码仓库及问题反馈
* https://github.com/Caihuining/Short-Semester/tree/main/style_transfer/fast_neural_style
## 参考
* https://github.com/onnx/models

