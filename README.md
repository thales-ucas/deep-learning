#  深度学习


本文章比较新手向，高手轻喷


## 下载anaconda


https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/


> anaconda包含python，并且可以创建多个环境


## 使用conda的清华源


原始的源在国外，比较慢，我们换成国内的源


打开“用户”目录下的“.condarc”，修改为下面内容
>  Windows 用户无法直接创建名为 “.condarc” 的文件，可先执行 ```conda config --set show_channel_urls yes``` 生成该文件之后再修改。


```yml
channels:
  - defaults
show_channel_urls: true
default_channels:
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/r
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/msys2
custom_channels:
  conda-forge: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  msys2: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  bioconda: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  menpo: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  pytorch: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  pytorch-lts: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  simpleitk: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
```


## 创建tensorflow环境


![环境](./docs/env.png)


现在可以激活这个环境


```bash
conda activate tf2
```


并且在这个环境下安装各种依赖库了


```bash
conda install tensorflow
```


## 打开这个项目的jupyter记事本


[./tape.ipynb](./tape.ipynb)


或者自己创建一个新的.ipynb文件


## 选择ipynb的核


![kernel](./docs/kernel.png)


现在可以运行每一行代码了


![run](./docs/run.png)