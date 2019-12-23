# 使用 AWS Deep Learning AMI  做文本分类

### Launch an AWS Deep Learning AMI


官方教程  [https://aws.amazon.com/cn/getting-started/tutorials/get-started-dlami/?nc1=h_ls](https://aws.amazon.com/cn/getting-started/tutorials/get-started-dlami/?nc1=h_ls)



### 配置 Jupyter Notebook



* Step 1  打开 **~/.jupyter/jupyter_notebook_config.py**, 设置配置文件   

```shell script
vim ~/.jupyter/jupyter_notebook_config.py
```


* Step 2 修改密码

```shell script
jupyter notebook password
```


* Step 3 配置其它信息
```python
## 服务的端口，用默认的8888即可
c.NotebookApp.port = 8888
 
## 是否需要自动弹出浏览器，服务器端一般不需要
c.NotebookApp.open_browser = False
 
## The directory to use for notebooks and kernels.
## 不设置的话就是启动命令所在的目录
c.NotebookApp.notebook_dir = '~/'

##  client ip 限制 
c.NotebookApp.ip='*'

```

###  配置 conda

```shell script

conda info --envs

source activate tensorflow_p36

pip install jieba

```
   


