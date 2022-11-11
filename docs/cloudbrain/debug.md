# 调试任务

> [!tip|icon:fa-solid fa-bars fa-bounce]
> - 在项目页面的 `云脑`->`调试任务`->`新建调试任务` 可以开启调试任务
> - 调试任务将启动 `镜像容器`，GPU任务与NPU任务的容器有着不同的层级构造
> - 调试任务将会在选择的镜像容器里提供 `Jupyter Lab` 控制台，你可以使用控制台里的 `Terminal` 管理镜像中的文件与Python库
> - 启动调试任务时，当状态由 `WAITING` 转为 `RUNNING` 后，需继续等待3-5分再点击 `调试` 跳转到控制台，提前点击 `调试` 会看到 `502错误界面`， 请退出并耐心等待

<!-- tabs:start -->

#### **GPU**

- 新建调试任务，计算资源选择 CPU/GPU ，并填写下列配置信息
    - 任务名称：只能包含 `小写字母，数字，以及下划线`
    - 镜像：可以选择任意 `平台镜像` 或者使用 `外部镜像`，粘贴镜像链接到框内即可
    - 数据集：点击 `选择数据集` 即可选择数据集
        - 数据集可 `多选` ，在弹窗中选中多个数据集即可
        - 你可以使用 `项目数据集` 或 `关联数据集`，你也可以在调试代码里下载 `外部数据集`
        - 此选项可以为 `空白` ，即不使用数据集
    - 资源规格：任意选择你想要的资源规格即可

<img src="_media/dataset/usagecreate.png" width = "800" alt="traindetail" align=middle />

<img src="_media/dataset/usagelab.png" width = "800" alt="traindetail" align=middle />

#### **NPU**


<!-- tabs:end -->