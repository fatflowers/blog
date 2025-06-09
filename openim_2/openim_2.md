# 独立部署openim遇到的坑（2）socket泄漏

> 公司项目有im场景，我们自己在k8s中部署了3.5.1版本的[openim](https://github.com/openimsdk)，在开发和运维的过程中，我们遇到了一些问题，这里记录一下问题详情和解决的过程。


## 问题触发场景
300个用户同时在线，并不定期单聊发送消息

## 问题现象
- 用户体感：发送消息后，收不到回复消息
- 从后端服务的角度：下发到openim的消息无法送达客户端
- 监控指标：
    - `openimserver-openim-push`容器cpu、内存上升很快
    - `openimserver-openim-push`和`openimserver-openim-msggateway` pod socket数很多
- 研发人员：手忙脚乱


https://github.com/openimsdk/helm-charts/blob/main/charts/openim-server/charts/openim-msggateway/templates/deployment.yaml
## 原因


## 解决办法


## 总结与反思
