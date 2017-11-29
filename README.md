## rtstool
* 此工具可以直接将已有的ceph卷导入到target中
* 请先安装和运行tcmu-runner，https://github.com/open-iscsi/tcmu-runner.git
## help：
```
<<<<<<< HEAD
[root@tcmu-runner-node rtstool-ceph]# ./rtstool.py 
Usage:
./rtstool.py create [name] [config] [size] [userid] [password] [iser_enabled] <initiator_iqn,iqn2,iqn3,...> [-a<IP1,IP2,...>] [-pPORT]
=======
[root@tcmu-runner-node rtstool]# ./rtstool.py 
Usage:
./rtstool.py create [device] [name] [userid] [password] [iser_enabled] <initiator_iqn,iqn2,iqn3,...> [-a<IP1,IP2,...>] [-pPORT]
./rtstool.py create_base_user_backstores [name] [config] [size] [userid] [password] [iser_enabled] <initiator_iqn,iqn2,iqn3,...> [-a<IP1,IP2,...>] [-pPORT]
>>>>>>> origin/rtstool-ceph-devel
./rtstool.py add-initiator [target_iqn] [userid] [password] [initiator_iqn]
./rtstool.py delete-initiator [target_iqn] [initiator_iqn]
./rtstool.py get-targets
./rtstool.py delete [iqn]
./rtstool.py verify
./rtstool.py save [path_to_file]
```
## example for create_base_user_backstores 
```
<<<<<<< HEAD
./rtstool.py create iqn.2017-10.com.redhat:c2596123456 rbd/volumes/ceph-block00 104857600 your_user_id your_passwd True iqn.1994-05.com.redhat:c25962a63511  -a192.168.88.58 -p3260
=======
./rtstool.py create_base_user_backstores iqn.2017-10.com.redhat:c2596123456 rbd/volumes/ceph-block00 104857600 your_user_id your_passwd True iqn.1994-05.com.redhat:c25962a63511  -a192.168.88.58 -p3260
>>>>>>> origin/rtstool-ceph-devel
```
