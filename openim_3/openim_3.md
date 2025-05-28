# 独立部署openim遇到的坑（3）扩容出错

> 公司项目有im场景，我们自己在k8s中部署了3.5.1版本的[openim](https://github.com/openimsdk)，在开发和运维的过程中，我们遇到了一些问题，这里记录一下问题详情和解决的过程。


## 触发场景
openimserver-openim-msggateway-0.openimserver-openim-msggateway-headless.eve-cn-infra-dev.svc.cluster.local

openim-push 
env
MY_MSGGATEWAY_REPLICACOUNT

这个变量需要与msggateway 数量一致

openimserver-openim-push-6f59668d9b-xdpcz 这个容器 cpu 内存上升很快

## 遇到的问题

## 原因


## 解决办法


## 反思
