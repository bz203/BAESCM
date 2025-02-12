# BAESCM

[简短描述你的项目和论文]

## 环境配置

1. 安装Miniconda/[Anaconda](https://www.anaconda.com/download)
2. 创建Conda环境：
   ```bash
   conda env create -f environment.yml
   conda activate your_env_name
   ```
3. 安装Earth Engine API并认证（geemap依赖）：
   ```bash
   earthengine authenticate
   ```

## 运行代码

1. 启动Jupyter Notebook：
   ```bash
   jupyter notebook
   ```
2. 打开 `notebooks/main.ipynb` 并运行。

## 常见问题
- **Geemap安装问题**：确保安装正确版本，建议 `conda install -c conda-forge geemap`
- **Earth Engine认证失败**：访问 [官方指南](https://developers.google.com/earth-engine/guides/python_install) 完成认证。
