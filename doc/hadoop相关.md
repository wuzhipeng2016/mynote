http://mirror.centos.org/altarch/7/isos/i386/

http://blog.csdn.net/fujianfafu/article/details/48577485
http://www.cnblogs.com/yunkaifa/p/4470422.html

http://blog.csdn.net/idber/article/details/40378231
centos
http://blog.csdn.net/kobe_lzq/article/details/7894718
centos download
https://www.centos.org/download/

http://www.cnblogs.com/HeroBeast/p/4962730.html
http://www.cnblogs.com/skyme/p/4606138.html
http://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-common/SingleCluster.html
http://hadoop.apache.org/releases.html#Download

rpm -qa|grep java
rpm -e --nodeps java-1.8.0-openjdk-1.8.0.65-3.b17.el7.x86_64
rpm -e --nodeps java-1.8.0-openjdk-headless-1.8.0.65-3.b17.el7.x86_64
oracle    mark200106/1234567
/home/java
rpm -ivh jdk-7u80-linux-x64.rpm 

增加用户
useradd -m hadoop -s /bin/bashadduser ha
cd ~/.ssh/ # 若没有该目录，请先执行一次ssh localhost
ssh-keygen -t rsa # 会有提示，都按回车就可以
cat ./id_rsa.pub >> ./authorized_keys # 加入授权
chmod 600 ./authorized_keys    #非常重要
ssh localhost

比较有用的安装
http://www.linuxidc.com/Linux/2014-10/108448.htm
    http://www.linuxidc.com/Linux/2014-10/108448p2.htm
http://www.cnblogs.com/hxbbing/p/4513184.html
http://www.powerxing.com/install-hadoop/
    http://www.powerxing.com/install-hadoop-in-centos/
http://www.open-open.com/lib/view/open1435761287778.html
http://blog.csdn.net/sxfcct/article/details/8469426

13、Web访问，要先开放端口或者直接关闭防火墙
(1)输入命令，systemctl stop firewalld.service
http://192.168.75.128:8088/cluster
http://192.168.75.128:50070/
http://192.168.75.128:9001


