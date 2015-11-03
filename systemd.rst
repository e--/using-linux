.. highlight:: bash

systemd
===============
systemd是linux最新的初始化系统

linux初始化系统是内核加之后执行的第一个程序，由这个程序进行后续环境的加载

主要命令
--------------

* systemctl
* journalctl

systemctl
-----------------
target maintenance::

    systemctl isolate multi-user.target

service lookup and maintenance::

    systemctl list-units --type service
    systemctl status mysql.service
    systemctl stop mysql.service
    systemctl start mysql.service
    systemctl disable mysql.service
    systemctl enable mysql.service

power management::

    systemctl reboot
    systemctl poweroff
    systemctl suspend
    systemctl hibernate
    systemctl hybird-sleep


