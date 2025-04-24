# Debug-date
## 导航调车日志
## 常用debug命令



## 编译
1. Libevent报错--源码下载---直接编译---CMAKE要重新学习
   
2. 库找不到，没安装，依赖有问题

2.1.[rosdep](https://fishros.org.cn/forum/topic/2124/rosdep%E6%98%AF%E4%BB%80%E4%B9%88-%E6%80%8E%E4%B9%88%E7%94%A8)
```python
# 安装rosdep-noetic
sudo apt-get install python3-rosdep
# 初次使用
sudo rosdep init
# 类似sudo apt-get update
rosdep update
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


