#   CastleX国赛程序更新
### 上下位通信功能包
(1)下载ros-melodic-castlex-bringup_amd64.deb包

(2)安装功能包
```bash
sudo dpkg -i ros-melodic-castlex-bringup_amd64.deb
roscd castlex_bringup/scripts/
sudo chmod +x *.py
```

(3)启动指令
```bash
roslaunch castlex_bringup castlex_stm32_bringup.launch
```

(4)话题说明



### 激光雷达功能包
(1)下载ros-melodic-arvlidar-ros_amd64.deb包

(2)安装功能包
```bash
sudo dpkg -i ros-melodic-arvlidar-ros_amd64.deb
```

(3)启动指令
```bash
roslaunch arvlidar_ros castlexlidar_A2.launch
```

(4)话题说明

### 语音系统功能包
(1)下载ros-melodic-castlex-voice-system_amd64.deb包

(2)安装功能包
```bash
sudo dpkg -i ros-melodic-castlex-voice-system_amd64.deb
roscd castlex_voice_system/scripts/
sudo chmod +x *.py
```

(3)启动指令
```bash
#   启动语音交互功能（需要联网）
roslaunch castlex_voice_system castlex_voice_system.launch

#   启动语音导航功能
roslaunch castlex_voice_system castlex_voice_nav.launch

#   启动语音抓取物体功能（桌面机械臂）
roslaunch castlex_voice_system castlex_voice_nav.launch

# 物联网相应功能
roslaunch castlex_voice_system castlex_iot.launch

# 消杀功能
roslaunch castlex_voice_system robot_xdu.launch
```

其他命令词自行修改launch文件中的bnf文件

### 物联网功能包
(1)下载ros-melodic-iot-wifi-system_amd64.deb包

(2)安装功能包
```bash
sudo dpkg -i ros-melodic-iot-wifi-system_amd64.deb
```

(3)启动指令
```bash
roslaunch castlex_voice_system castlex_iot.launch
```


