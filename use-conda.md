---
title: "软件使用"
date: 2018-07-09T20:31:49+08:00
draft: false
---

# 用conda创建python虚拟环境
##

- conda list 查看安装了哪些包
- conda env list 或 conda info -e 查看当前存在哪些虚拟环境


    conda create -n your_env_name python=X.X

## 将anaconda的环境添加到jupyter中

1. 进入anaconda的一个环境
2. 安装 ipykernel
    ```
    pip install ipykernel
    #or
    conda install ipykernel
    ```
3. 将本环境添加到jupyter中
    ```
    python -m ipykernel install --user
    #or
    ipython kernel install --user
    source activate myenv
    python -m ipykernel install --user --name myenv --display-name "Python (myenv)"

    ```

- 查看当前kernel
    ```
    jupyter kernelspec list
    ```
- 删除notebook kernel
    ```
    jupyter kernelspec remove kernelname
    ```
- 搜xmltodict包
```
anaconda search -t conda xmltodict
conda create -c rdkit -n my-rdkit-env rdkit
conda install scikit-learn
```
