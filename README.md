# fas-notebooks

本仓库存放有在学习[火灾预警系统](https://fas.coding.net)开发中用到的机器学习等知识时整理出的笔记，以 Jupyter Notebooks 的形式呈现。

> 如果还不熟悉 Jupyter Notebook，建议选择下文中的 [`在线运行`](#在线运行) 后进入笔记本 `Jupyter Notebook 简介.ipynb` 简单了解一下。

## 如何运行

### 本机运行（推荐）

如果已经配置了 Python 运行环境，不妨在本机[安装 Jupyter Notebook](https://jupyter.org/install)，再将此仓库克隆或下载（点击右上方 `Clone or Download` 按钮）到本机运行。

在打开笔记本之前，在克隆或下载的本仓库目录下运行以下命令以安装所用到的库（NumPy、Matplotlib 等）：

```bash
conda env create -f conda/environment.yml
```

> 1. 应当使用 `conda/environment.yml` 而非 `environment.yml`：后者是为在线运行（[Binder](https://mybinder.org/)，服务器在国外）准备的，它们唯一的区别为 `conda/environment.yml` 使用了国内镜像而 `environment.yml` 使用的是官方源；
>
> 2. 如果没有 Anaconda 或认为 Anaconda 安装太慢，可以使用 `pip` 代替，本仓库中也为 `pip` 提供了相应的配置文件。运行以下命令：
>
>    ```bash
>    pip install -r pip/requirements.txt
>    ```
>
>    **`pip` 无法自动安装 PyTorch；安装 PyTorch 需要使用 Anaconda 或手动下载安装包。**

### 在线运行

点击下面的按钮或[此链接](https://mybinder.org/v2/gh/YangHanlin/fas-notebooks/master)可以在线运行本仓库中的 Jupyter Notebooks，使用体验取决于网络环境。

[![使用 Binder 运行](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/YangHanlin/fas-notebooks/master)

> **在线查看：** 如果只想要预览笔记，无需运行，可以直接在 GitHub 中点击文件名预览，也可以点击[此链接](https://nbviewer.jupyter.org/github/YangHanlin/fas-notebooks/tree/master/)。