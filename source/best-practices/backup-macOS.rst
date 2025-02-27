macOS 数据备份
--------------

:本节贡献者: |田冬冬|\（作者）、
             |姚家园|\（作者）
:最近更新日期: 2021-10-01
:预计阅读时间: 20 分钟

----

Time Machine
^^^^^^^^^^^^

macOS 下最好用的备份工具当属 Time Machine（时间机器），其可以增量备份 macOS 下的文件，
能恢复到之前任意备份时刻的状态，并且操作简单。当然也可以使用 ``rsync`` 命令进行备份，
与 Linux 下相同。推荐使用 Time Machine 进行备份。

首先插入一块备用硬盘，按下 :kbd:`Command` + :kbd:`空格`，搜索“Disk Utility”并按下
:kbd:`Enter` 键以打开磁盘工具。将移动硬盘格式化成 APFS（加密）格式，这也是 macOS Big Sur（11.x）
的默认格式。读者可以根据自身情况选择分区大小，推荐至少是 macOS 本身硬盘空间的两倍。

点击左上角的 Apple 图标，在“系统偏好设置”中，打开“时间机器”。选中“在菜单栏中显示时间机器”。
点击“选择备份磁盘”，从可用磁盘列表中选择之前格式化的硬盘分区，然后选择“使用磁盘”即可。
时间机器会立即开始备份。首次备份可能需要很长时间，之后只会同步有改动的文件。下次插入备份硬盘，
直接从菜单栏的时间机器菜单中选择“立即备份”即开始增量备份。可以选择“进入时间机器”，查看备份内容。
如需还原备份文件，请参考官方支持\ `从备份恢复 Mac <https://support.apple.com/zh-cn/HT203981>`__。
