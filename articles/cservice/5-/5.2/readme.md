# 服务发现

## 功能简介

用友云服务发现是服务注册中心核心功能之一, 服务发现组件记录了（大规模）分布式系统中所有服务的信息，其它服务可以据此找到这些服务。服务发现组件提供了很多的功能，例如，服务元数据存储、健康监控、多种查询和实时更新等。


![](image/service-discover.png)

## 主要特征

- 服务提供者的实例在启动时或者位置信息发生变化时会向服务注册表注册自身，在停止时会向服务注册表注销自身，如果服务提供者的实例发生故障，在一段时间内不发送心跳之后，也会被服务注册表注销。

- 服务消费者的实例会向服务注册表查询服务提供者的位置信息，然后通过这些位置信息直接向服务提供者发起请求。

- 发起请求时会可使用多种负载均衡策略, 如:hash, 权重, 响应时间等.


## 接入步骤
- 参见"服务注册中心"文档.
