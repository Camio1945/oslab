# oslab

压缩包 `oslab.zip` 是[蓝桥云课：操作系统原理与实践](https://www.lanqiao.cn/courses/115)的实验环境中的 `/home/shiyanlou/oslab` 文件夹打包而来的，方便大家在虚拟机上测试。

步骤：

1. 使用虚拟机软件（如 VMware ）创建虚拟机（如 Ubuntu 23.04），需要是桌面版的虚拟机，不能是服务器版的虚拟机，因为依赖了桌面环境的 bochs 。

2. 需要创建一个名为 `shiyanlou` 的账号，该账号对应的 home 目录路径应该为： `/home/shiyanlou` 

3. 下载 `oslab.zip` ，放到 `/home/shiyanlou/` 目录下并解压。

4. 两步调试
	
	1.  	在桌面环境下，打开终端，进入 `/home/shiyanlou/oslab/` 后运行 `./dbg-c` 。
	2.  	打开另一个终端（可以是 ssh 连接的终端），进入 `/home/shiyanlou/oslab/` 后运行 `./rungdb` 。