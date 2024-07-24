# bitlocker-autolock
bitlocker autolock 自动锁定
能够实现让电脑睡眠/休眠/锁定后自动锁定bitlocker加密盘

打开lockdrive.bat
在第二行修改需要自动锁定的硬盘
win+R 输入taskschd.msc并打开
点击创建任务
- 常规 填写*任务名称* 并且选择*使用最高权限运行*
- 触发器 选择*登录时* 其余全部默认即可
- 操作
