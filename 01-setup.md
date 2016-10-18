# 安装与配置

R的安装配置包括几个方面：
* windows环境下状态
* Linux环境下安装
* Mac 下安装
* R 基础配置内容
* RStudio 安装与配置使用
* 新R环境，第三方包快速复制方法

## windows 环境下安装

window环境下安装需要注意点：
* 不要安装在中文目录下
* 尽量需要选择默认的中文语言环境（翻译很烂，难以看懂），遇到问题大多需要到stackflow上找答案，中文都无法及时找到可靠答案）
* 

## Linux环境下安装

### centos 安装R

centos下安装比较麻烦，主要还牵涉到软件库的寻找较为麻烦，经过测试验证，下述方式是可以正确使用的，可以安装到较新的R版本.

1. 运行 yum list R-\*，查看结果
对应的软件安装源是否存在R的安装包，对应的版本是否为最新的
目前最新的是3.3.1
若存在，且为最新的

2. 若没有则可以使用这个软件源来安装最新的R包
版本不同可以参考：
>$ https://fedoraproject.org/wiki/EPEL/FAQ#How_can_I_install_the_packages_from_the_EPEL_software_repository.3F
 
 >$ su -c 'rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm'
$ yum list R-\*

3. 安装R包：
> $ yum install R

4. 安装第三方包：
1）install.packages('Rserve')
按照完毕之后 library(Rserve) 查看是否报错，没有报错则按照完毕正常
2）install.packages('forecast')按照预测使用的包
若不正常，则查看是哪个依赖的包报错的，然后单独安装该包，看具体报错是什么，然后再跟进具体的报错情况，来查找具体的解决方案。

5. 注意事项：

> * centos尽量使用7以上版本，若使用6版本的，可能在安装第三方包的时候会出现很多兼容问题（截止2016.10）.
> * 安装过程需要全程联网，且最好能够访问国外网站（墙） 


## Mac 下安装

没有尝试过，暂时未知

## R 基础配置内容

## RStudio 安装与配置使用

作为最为专业，常用的R语言的IDE，Rstudio无疑是我们的最好助手。

### 下载安装

### 功能简介

### 环境配置
