## rtstool-ceph
* 此工具可以直接将已有的ceph卷导入到target中
* 请先安装和运行tcmu-runner，https://github.com/open-iscsi/tcmu-runner.git
## 使用举例
* 创建target,用法如下：
```
./rtstool-ceph.py create [name] [config] [size] [userid] [password] [iser_enabled] <initiator_iqn,iqn2,iqn3,...> [-a<IP1,IP2,...>] [-pPORT]
```
* create命令使用举例
```
./rtstool-ceph.py create iqn.2017-10.com.redhat:c2596123456 rbd/volumes/ceph-block00 104857600 your_user_id your_passwd True iqn.1994-05.com.redhat:c25962a63511
```
