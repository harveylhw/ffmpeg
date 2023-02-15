# FFmpeglive
ffmpeg实现24小时不间断推流
功能：

1.支持循环推流mp4格式的视频，视频文件的名字不能含有空格或其他特殊符号。

2.视频加水印，水印位置默认在右上角。

需要配合screen运行：
```
yum -y install screen
```
开个新窗口：
```
screen -S stream
```
创建目录ffmpeg：
```
mkdir /home/你自己的用户名/ffmpeg
```
进入ffmpeg目录：
```
cd /home/你自己的用户名/ffmpeg
```

查看进程：
```
screen -ls
```
开启后台运行进程：
```
screen -d 进程名
```
关闭后台运行进程：
```
screen -X -s 进程名 quit
```
执行FF_Live：
```
bash <(curl -Ls https://raw.githubusercontent.com/harveylhw/FFmpeg/main/start.sh)
```
