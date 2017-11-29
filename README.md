## rtstool-ceph
* 此工具可以直接将已有的ceph卷导入到target中
* 请先安装和运行tcmu-runner，https://github.com/open-iscsi/tcmu-runner.git
## 使用举例
* 创建target,用法如下：
```
[root@tcmu-runner-node rtstool-ceph]# ./rtstool-ceph.py 
Usage:
./rtstool-ceph.py create [name] [config] [size] [userid] [password] [iser_enabled] <initiator_iqn,iqn2,iqn3,...> [-a<IP1,IP2,...>] [-pPORT]
./rtstool-ceph.py add-initiator [target_iqn] [userid] [password] [initiator_iqn]
./rtstool-ceph.py delete-initiator [target_iqn] [initiator_iqn]
./rtstool-ceph.py get-targets
./rtstool-ceph.py delete [iqn]
./rtstool-ceph.py verify
./rtstool-ceph.py save [path_to_file]
```
* create命令使用举例
```
./rtstool-ceph.py create iqn.2017-10.com.redhat:c2596123456 rbd/volumes/ceph-block00 104857600 your_user_id your_passwd True iqn.1994-05.com.redhat:c25962a63511  -a192.168.88.58 -p3260
```
