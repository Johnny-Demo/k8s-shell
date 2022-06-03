# k8s-shell
注意事项：
一、selinux 脚本单独执行，selinux 关闭之后要重启服务器才能生效。
二、除了执行 reset.sh 脚本以外，其他脚本执行之前都要先修改里面的 ip，根据自己情况删除或者添加。
三、执行 install.sh 需要根据自己情况修改里面的 k8s 镜像源和仓库，k8s 版本号。
四、执行脚本顺序
1、selinux.sh（执行完需要重启所有节点服务器）
2、env.sh
3、ha.sh
4、install.sh
5、reset.sh（如果初始化集群有问题可以直接执行，没必要的情况下可以不执行。） 
