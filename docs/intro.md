> [!tip| label: 加入我们！|icon:fa-solid fa-envelope fa-bounce]
> 现在就加入启智社区，尽享普惠算力。[立即注册](https://git.openi.org.cn/user/sign_up)

### 平台介绍

> [!note|label:启智社区|icon:fas fa-house]
> `启智AI开发协作平台`，简称 `启智社区` ，是一个开源在线Web应用，旨在为人工智能算法、模型开发提供在线协同工作环境，它提供了代码托管、数据集管理与共享、免费云端算力资源支持(GPU/NPU)、共享镜像等功能。启智社区是基于Gitea发展而来的，我们对其进行了Fork并基于此扩展了人工智能开发中需要的功能，如数据集管理和模型训练等。对于和代码托管相关的功能，您可以参考Gitea的文档。

<img src="_media/openi/HOME0.png" width = "800" alt="homepage" align=center />



### 功能介绍

在启智开源社区里，`项目`是基础。你将在`项目`下提交代码，上传数据集，调试代码，创建镜像，训练模型，以及管理模型。

- **个人中心:** 用户中心里，你能快速查看自己参与的项目，待处理的任务以及所有的云脑任务列表。

- **项目:** 项目的核心是代码仓，所有的代码文件都将提交到代码仓。如果你还不熟悉Git操作，可以参考[此篇教程](https://www.runoob.com/git/git-tutorial.html)。

- **数据集:** 每个项目只能创建一个数据集，但你可以在里面上传多个打包文件。除此之外，你还可以公开数据集。公开的数据集会在导航栏的数据集里显示。

- **模型:** 你可以在启智社区保存的你模型。导航栏的模型下提供了模型体验功能。

- **探索:** 在探索功能下，你可以查看其他用户，组织，以及云脑镜像。

###  资源说明

<!-- tabs:start -->

#### **🐶启智集群**
<!-- tabs:start -->
#### **🐶GPU**
| 任务类型 | 卡类型 | 可用镜像 |  网络类型 |数据集处理方式|容器目录说明|
|---------|:-|:------:|:------:|:--------|:------------|
| 调试任务 | T4 |外部公开镜像，如dockerhub镜像；平台镜像；| 能连外网|平台解压数据集| 数据集存放路径/dataset，模型存放路径/model，代码存放路径/code |
| [训练任务](https://git.openi.org.cn/OpenIOSSG/MNIST_PytorchExample_GPU) | V100 |	平台镜像；| 不能连外网|平台解压数据集| 训练脚本存储在 /code 中，数据集存储在 /dataset 中，预训练模型存放在运行参数 ckpt_url 中，训练输出请存储在 /model 中以供后续下载。 |
| [训练任务](https://git.openi.org.cn/OpenIOSSG/MNIST_PytorchExample_GPU) | A100 |外部公开镜像，如dockerhub镜像；平台镜像；| 能连外网|平台解压数据集| 训练脚本存储在 /code 中，数据集存储在 /dataset 中，预训练模型存放在运行参数 ckpt_url 中，训练输出请存储在 /model 中以供后续下载。 |
| [推理任务](https://git.openi.org.cn/OpenIOSSG/MNIST_PytorchExample_GPU/src/branch/master/inference.py)	 | V100 | 平台镜像；| 不能连外网 |平台解压数据集| 数据集存储在 /dataset 中，模型文件存储在 /model 中，推理输出请存储在 /result 中以供后续下载。 |
| [评测任务](https://git.openi.org.cn/OpenIOSSG/aisafety)	 | V100 | 平台镜像；| 不能连外网 |平台解压数据集|  |
>[!warning|label:备注|icon:fa-sharp fa-solid fa-pen]
>启智集群V100不能连外网，只能使用平台的镜像，不可使用外部公开镜像，否则任务会一直处于waiting状态
#### **🐶NPU**
| 任务类型 | 卡类型 | 可用镜像 |  网络类型 |数据集处理方式|容器目录说明|
|---------|:-:|:------:|:------:|:--------|:------------|
| 调试任务 | Ascend 910 | 平台镜像；| 能连外网|平台解压数据集,但需要自己拷贝到容器中。| |
| [训练任务](https://git.openi.org.cn/OpenIOSSG/MNIST_Example) | Ascend 910 |	平台镜像；| 能连外网|平台解压数据集,但需要自己拷贝到容器中。| 数据集位置存储在运行参数 data_url 中，预训练模型存放在运行参数 ckpt_url 中，训练输出路径存储在运行参数 train_url 中。 |
| [训练任务](https://git.openi.org.cn/OpenIOSSG/MNIST_Example) | Ascend 910 |平台镜像；| 能连外网|平台解压数据集,但需要自己拷贝到容器中。| 数据集位置存储在运行参数 data_url 中，预训练模型存放在运行参数 ckpt_url 中，训练输出路径存储在运行参数 train_url 中。 |
| [推理任务](https://git.openi.org.cn/OpenIOSSG/aisafety)	 | Ascend 910 | 平台镜像；| 能连外网 |平台解压数据集,但需要自己拷贝到容器中。|  
<!-- tabs:end -->

#### **🐱智算集群**
<!-- tabs:start -->
#### **🐱GPU**
| 任务类型 | 卡类型 | 可用镜像 |  网络类型 |数据集处理方式|容器目录说明|
|--------------|:-:|:------:|:------:|:--------|:---------|
| [训练任务](https://git.openi.org.cn/OpenIOSSG/MNIST_PytorchExample_GPU/src/branch/master/train_for_c2net.py) | V100 |	外部公开镜像，如dockerhub镜像；平台镜像；| 不能连外网|用户自行解压数据集| 训练脚本存储在 /tmp/code 中，数据集存储在 /tmp/dataset 中，预训练模型存放在运行参数 ckpt_url 中，训练输出请存储在 /tmp/output 中以供后续下载。 |
| [训练任务](https://git.openi.org.cn/OpenIOSSG/MNIST_PytorchExample_GPU/src/branch/master/train_for_c2net.py) | A100 |	外部公开镜像，如dockerhub镜像；平台镜像；| 能连外网|用户自行解压数据集| 训练脚本存储在 /tmp/code 中，数据集存储在 /tmp/dataset 中，预训练模型存放在运行参数 ckpt_url 中，训练输出请存储在 /tmp/output 中以供后续下载。 |
>[!warning|label:备注|icon:fa-sharp fa-solid fa-pen]
>启智集群V100不能连外网，只能使用平台的镜像，不可使用外部公开镜像，否则任务会一直处于waiting状态
#### **🐱NPU**
| 任务类型 | 卡类型 | 可用镜像 |  网络类型 |数据集处理方式|容器目录说明|
|--------------|:-:|:------:|:------:|:---------|:---------|
| [训练任务](https://git.openi.org.cn/OpenIOSSG/MNIST_Example/src/branch/master/train_for_c2net.py) | Ascend 910 |平台镜像；| 能连外网|用户自行解压数据集| 训练脚本存储在 /tmp/code 中，数据集存储在 /训练脚本存储在 /cache/code 中，预训练模型存放在运行参数 ckpt_url 中，训练输出请存储在 /cache/output 中以供后续下载。 |
<!-- tabs:end -->

<!-- tabs:end -->