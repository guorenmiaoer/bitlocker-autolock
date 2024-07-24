# bitlocker-autolock
bitlocker 自动锁定
能够实现让电脑睡眠/休眠/锁定后自动锁定bitlocker加密盘

1. 打开 `lockdrive.bat` 文件。
2. 在第二行修改需要自动锁定的硬盘盘符。
3. 按 `Win + R` 键，输入 `taskschd.msc`，然后按回车键打开任务计划程序。
4. 点击“创建任务”：
   - **常规**：填写*任务名称*，并选择*使用最高权限运行*。
   - **触发器**：选择*登录时*，其余设置保持默认，或根据需要进行配置。
   - **操作**：点击“新建”，在*程序或脚本*字段中选择 `lockdrive.bat` 脚本。
5. 点击“确定”保存任务。

To automatically lock a BitLocker-encrypted drive when the computer goes to sleep, hibernates, or locks:

1. Open `lockdrive.bat`.
2. On the second line, modify the drive letter for the drive you want to automatically lock.
3. Press `Win + R`, type `taskschd.msc`, and press Enter to open Task Scheduler.
4. Click "Create Task":
   - **General**: Enter a *task name* and select *Run with highest privileges*.
   - **Triggers**: Select *At log on*; leave the other settings as default or configure as needed.
   - **Actions**: Click *New*, then select your `lockdrive.bat` script under *Program/script*.
5. Click OK to save the task.
