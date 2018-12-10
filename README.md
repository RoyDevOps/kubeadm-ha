# install

![](https://img.shields.io/badge/Dist-Centos7-blue.svg) ![](https://img.shields.io/badge/Dist-Fedora27-yellow.svg) ![](https://img.shields.io/badge/DNS-CoreDNS-brightgreen.svg)  ![](https://img.shields.io/badge/Mode-HA-brightgreen.svg)  ![](https://img.shields.io/badge/Proxy-IPVS-brightgreen.svg)  ![](https://img.shields.io/badge/Net-Calico-brightgreen.svg)

``` shell
# 创建集群信息文件
$ cat ./cluster-info
CP0_IP=10.130.29.80
CP1_IP=10.130.29.81
CP2_IP=10.130.29.82
VIP=10.130.29.83
NET_IF=ens32
CIDR=10.244.0.0/16

$ bash -c "$(curl -fsSL https://k8s.lentil1016.cn)"
```

## generate join command

``` shell
kubeadm token create --print-join-command
```
