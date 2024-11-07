# slam-14-lecture-learning
高翔老师的slam十四讲学习仓库，ros版本

## 一、安装说明

### 1、docker

默认已经安装完成docker, 如果没有, 请参考[官方文档](https://docs.docker.com/desktop/install/linux/ubuntu/):
docker镜像国内源配置: 

```shell
vim /etc/docker/daemon.json 

# 文件中输入，文件不存在就创建。
{
    "registry-mirrors": [
    "https://2a6bf1988cb6428c877f723ec7530dbc.mirror.swr.myhuaweicloud.com",
    "https://docker.m.daocloud.io",
    "https://hub-mirror.c.163.com",
    "https://mirror.baidubce.com",
    "https://your_preferred_mirror",
    "https://dockerhub.icu",
    "https://docker.registry.cyou",
    "https://docker-cf.registry.cyou",
    "https://dockercf.jsdelivr.fyi",
    "https://docker.jsdelivr.fyi",
    "https://dockertest.jsdelivr.fyi",
    "https://mirror.aliyuncs.com",
    "https://dockerproxy.com",
    "https://mirror.baidubce.com",
    "https://docker.m.daocloud.io",
    "https://docker.nju.edu.cn",
    "https://docker.mirrors.sjtug.sjtu.edu.cn",
    "https://docker.mirrors.ustc.edu.cn",
    "https://mirror.iscas.ac.cn",
    "https://docker.rainbond.cc"
    ]
}
```

docker镜像

```shell
docker pull osrf/ros:noetic-desktop-full
```

### 2、ros配置

通过osrf/ros:noetic-desktop-full镜像创建的容器需要安装其它环境（不包含一般工具，如git等）

```shell
sudo apt-get install ros-noetic-moveit
```

