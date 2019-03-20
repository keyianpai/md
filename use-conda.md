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
- 常用命令
```sh
jupyter notebook
jupyter nbextension enable codefolding/main
jupyter notebook --ip=10.20.2.20
nohup jupyter notebook --ip=10.20.2.20 > jupyterout817  2>&1 &
jobs -l #列出后台进程
watch -n 10 nvidia-smi #每10秒执行一次NVIDIA命令

jupyter lab --ip=10.20.2.20
source activate rdk-27
source deactivate rdk-27
tar -zvxf example.tar.gz
tar -jxvf xx.tar.bz2
rar a etc.rar /etc
$xz -d ***.tar.xz
$tar -xvf  ***.tar
#将/etc 目录压缩为etc.rar
# 解压，加v表示verbose
.gz
　　解压 1：gunzip FileName.gz 
　　解压2：gzip -d FileName.gz
import os
from os.path import join, getsize
for root, dirs, files in os.walk('.'):
    print("{}:\n{}\n{}\n".format(root,dirs,files))
D:\Program Files (x86)\Common Files\Oracle\Java\javapath
```
安装Tomcat，闪退，各种配环境变量，都是闪退，事实上只需要配置CATALINA_HOME就够了，重要的是重启一下电脑。
```
在postgres中查询用户

select* from pg_user;
查询系统中的数据库
select* from pg_database;
Create database i2b2demodata；
#注意引号，且必须是单引号
postgres# CREATE USER xxxx1 WITH PASSWORD 'xxxx';
CREATE USER i2b2hive WITH PASSWORD 'demouser';
CREATE ROLE name PASSWORD 'string';
CREATE ROLE i2b2imdata CREATEDB PASSWORD 'demouser';
CREATE ROLE i2b2workdata CREATEDB LOGIN PASSWORD 'demouser';
postgres# CREATE DATABASE xxxx2;
postgres# GRANT ALL PRIVILEGES ON DATABASE xxxx2 to xxxx1;
#改变数据库拥有者,把x2给x1
alter database xxxx2 owner to xxxx1;
#列出所有用户
\du
#赋予用户创造数据库权限
ALTER ROLE i2b2hive createdb;
\password
https://blog.csdn.net/u010166404/article/details/53188882
```

dos中
```
createuser –help
# 用超级用户postgres创建新用户，并赋予创建数据库权限
createuser -U postgres -d i2b2demodata
```
static means this method belongs to the class Main and not to a specific instance of Main
result = re.sub('abc',  '',    input)           # Delete pattern abc
http://www.learnjavaonline.org/en/Functions
参数传递时，原子类型与对象表现不同，原子类型复制了一个副本，对象则不是
But when we assign objects, it's a bit different than assigning primitives.
Non static methods in Java are used more than static methods. Those methods can only be run on objects and not on the whole class.

Every Java method has to be within a class
Static methods belong to a class while non-static methods belong to objects
All parameters to functions are passed by value, primitives content is copied, while objects are not copied and some would say 'passed by reference'

When using the keyword private before a variable or a method, it means only the class itself can access the variable or method, when we're using public it means everybody can access it. We usually see constructors defined as public, variables defined as private and methods are separated, some public and some private.

the term inheritance refers to the adoption of all non-private properties and methods of one class (superclass) by another class (subclass). Inheritance is a way to make a copy of an existing class as the starting point for another.
subclass, derived classes

The methods and properties of a subclass can be used just like those of it's superclass. They can also be overridden. Overriding is the process of replacing (or augmenting) the original code with new code to suit the current purpose.


Abstract classes can contain fields which are not final and static and can contain implemented methods as well but interfaces cannot. Abstract classes with only abstract methods should be defined as interfaces.

Interfaces define methods for classes by specifying the method name, the return type (or void) and the method arguments (by type and name). These method definitions are called signatures. Because this is a template, the method signatures contain no code. The code is entered into the implementation of an interface. Interfaces are used in the discipline of polymorphism.

java运行包时应注意加上目录名，否则就会出现 找不到或无法加载主类 MammalInt的情况。
java animals/MammalInt
