# Integrated_Practice_of_Embedded_Systems
Atlas 200DK 嵌入式系统实验

2021年秋季课程大作业
基于串口的IM通信系统


环境配置： Ubuntu 16.04
依赖包：   socat
安装方式 apt-get install socat
apt-get install socat

## 使用方法
1.开启两个固定虚拟串口 
socat -d -d pty,b115200 pty,b115200
/dev/ttyS10 , /dev/ttyS11

`bash socatopenport.sh`

2.分别在两个终端启动程序

`python3 main.py userinfo1.json`

`python3 main.py userinfo2.json`

3.在shell中输入信息即可发送

发送文件时前缀为 `file:`
