# KBI
Kubernetes Binarization Installer 
## 运行方法
```shell
bash kbi.sh -i
# 或者
chmod a+x kbi.sh
./kbi.sh -i
# 根据提示进行操作即可，注意，输入时不能携带特殊字符
```
- 输入IP和K8s版本，即可完成K8s二进制高可用安装（含Ingress-Controller和CoreDNS）;
- 最少要求3个节点，即3个Master同时作为Node来部署，要求宿主机系统版本为RHEL 7/CentOS 7;
- 理论上1.13之后的所有版本都可以安装，如果你想要的小版本在OSS中不存在，可以联系我或者你也可以自行下载server类型的tar.gz分发包，解压至所有节点的/usr/local/bin目录下，脚本检测到存在kube-apiserver文件则跳过下载kubernetes-server-XXX.tar.gz文件的步骤;
），已上传至OSS的版本如下：
> - 1.16.15
> - 1.17.14
> - 1.18.10
> - 1.19.4


