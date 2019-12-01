+ [linux根文件系统 /etc/resolv.conf 文件详解](https://blog.csdn.net/mybelief321/article/details/10049429)

+ [常用dns114.114.114.114与8.8.8.8的区别](https://blog.csdn.net/zhezhebie/article/details/79191776)

+ [Linux 命令详解（三）./configure、make、make install](https://www.cnblogs.com/tinywan/p/7230039.html)

+ [Mysql配置文件/etc/my.cnf解析](https://www.jianshu.com/p/5f39c486561b)

+ [Linux unZip/Zip的安装及使用](https://www.jianshu.com/p/29e15cd4afcc)

+ [Linux 压缩包解压后撤销(undo unzip & tar)](https://www.jianshu.com/p/777c2a0f16b4)

		zipinfo -1 path/xx.zip | xargs rm -rf
		
		tar -tf xx.tar | xargs rm -rf
		eg: tar -tf war5.0.tgz | xargs rm -rf
+ [vim常用命令之多行注释和多行删除](https://blog.csdn.net/helloxiaozhe/article/details/78562359)

+ [systemctl命令完全指南](https://linux.cn/article-5926-1.html)

+ [Linux软件安装管理之——RPM与YUM详解](https://segmentfault.com/a/1190000011200461)

+ [分布式系统服务单点问题的探讨](https://www.jianshu.com/p/91d0950785b4)

+ Linux更改系统时区


	vim /etc/sysconfig/clock  
	写入ZONE=Asia/Shanghai
	rm /etc/localtime
	ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
	yum -y install tzdata
	查看当前时间 date
	安装模块：yum install -y ntp
	更新时间 ntpdate time.windows.com
	vi   /etc/crontab 写入：* * * * * root ntpdate time.windows.com
	
+ [ps -ef|grep详解](https://www.cnblogs.com/freinds/p/8074651.html)

	查找一个字段出现的位置  grep -r "" *
	
	替换该文件中的该字段 %s/old/new/g
	查看某个进程
	ps -ef|grep 
	
+ [在Linux中终止进程的Kill，Pkill和Killall命令指南](https://www.howtoing.com/how-to-kill-a-process-in-linux)
+ [如何查看Linux服务器中所有正在运行的进程服务？](https://yq.aliyun.com/articles/690005)
+ [ntp服务器](http://cn.linux.vbird.org/linux_server/0440ntp.php#client_linux)
+ [vim 全局替换](https://blog.csdn.net/shuangde800/article/details/10554513)

	将文件中所有old替换为new
	:/s/old/new/g


