# Ubuntu自动定时关机的方法

[sudo] shutdown 参数 延迟时间

在终端输入：
sudo shutdown +100      就表示电脑在100分钟后关机。

-k              并不真正关机而只是发出警告信息给所有用户

-r  now         现在立即重新启动
-r +3           三分钟后重启
-r 20:23        在20：23时将重启计算机
-r 20:23 &      将20：23时重启的任务放到后台去，用户可以继续操作终端

-h  now         现在立刻关机
-h +3           三分钟后关机
-h 12:00        在12点关机

-f              快速关机重启动时跳过fsck
-n              快速关机不经过init程序。(不推荐)

如果你此时手动关机是没用的，关机和重启都会变成登出，
可以用 sudo shutdown -c来取消自动关机的命令。
