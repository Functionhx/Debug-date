# Debug-date
## 导航调车日志
## 常用debug命令
```cpp
rosrun rqt_tf_tree rqt_tf_tree
rosrun rqt_configure rqt_configure
```
```
rqt
rqt_graph
```
```
rostopic list
rostopic echo <ros_topic_name>
rostopic info <ros_topic_name>
rosservice list
rosaction list
```
```
rostopic pub -r 10 /cmd_vel tab tab tab
```
```
rosnode list
rosnode info <node_name>
```
## 局部规划器插件流程

## 编译
1. Libevent报错--源码下载---直接编译---CMAKE要重新学习
   
2. 库找不到，没安装，依赖有问题

不能跨包include，除非会写cmake 

3. 库没安装

2.1.[rosdep](https://fishros.org.cn/forum/topic/2124/rosdep%E6%98%AF%E4%BB%80%E4%B9%88-%E6%80%8E%E4%B9%88%E7%94%A8) 下载国外镜像，可能有问题
```python
# 安装rosdep-noetic
sudo apt-get install python3-rosdep
# 初次使用
sudo rosdep init
# 类似sudo apt-get update
rosdep update
```
2.2 [rosdepc](https://zhuanlan.zhihu.com/p/398754989) 这是鱼香ros做的gitee版
```python
# 安装rosdep-noetic
sudo apt-get install python3-pip  # 若无pip工具
sudo pip install rosdepc
# 初次使用
sudo rosdepc init
# 类似sudo apt-get update
rosdepc update
```
## 通信
**串口连接不上:**
1. chmod 串口权限
2. lsusb 查看是否STM32连上串口

**雷达连接不上**
1. 以太网网络配置
2. ws_livox-config

**打点导航不动**
1. 检查雷达SLAM算法启动是否成功
2. 雷达扫描的地图是否加载成功
3. 
**导航有问题**
1.先查通信是否存在问题


