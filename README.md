# oslab

压缩包 `oslab.zip` 是[蓝桥云课：操作系统原理与实践](https://www.lanqiao.cn/courses/115)的实验环境中的 `/home/shiyanlou/oslab` 文件夹打包而来的，方便大家在虚拟机上测试。

步骤：

1. 使用虚拟机软件（如 VMware ）创建虚拟机，虚拟机镜像文件推荐使用 [ubuntu-12.04.4-desktop-i386.iso](http://old-releases.ubuntu.com/releases/12.04/ubuntu-12.04.4-desktop-i386.iso)，因为原实验环境中就是用的 ubuntu12.04 桌面版，而且依赖了 32 位的软件。

2. 需要创建一个名为 `shiyanlou` 的账号，该账号对应的 home 目录路径应该为： `/home/shiyanlou` 

以 ubuntu 为例，创建用户相关的命令如下（一行一行执行，因为中间需要设置密码）：
```sh
sudo useradd shiyanlou
sudo passwd shiyanlou
设置密码、确认密码，可以设置为 shiyanlou 
sudo mkdir /home/shiyanlou
sudo chown -R shiyanlou:shiyanlou /home/shiyanlou
sudo chsh -s /bin/bash shiyanlou
```

3. 用 shiyanlou 这个账号登录。
4. 下载 `oslab.zip` ，放到 `/home/shiyanlou/` 目录下并解压。(上传文件到虚拟机可以使用 VMware tools 工具)
5. 在桌面环境下，打开终端，进入 `/home/shiyanlou/oslab/` 后运行 `./dbg-c` 。
6. 打开另一个终端（可以是 ssh 连接的终端），进入 `/home/shiyanlou/oslab/` 后运行 `./rungdb` 。