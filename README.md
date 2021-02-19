# Introduction

Prometheus是一套开源监控报警系统（包括时序列数据库TSDB），自2012年来被许多公司与组织所采用。其中Prometheus的特点如下：

多维数据模型（时序列数据由metric名和一组key/value组成）
在多维度上灵活的查询语言(PromQL)
不依赖分布式存储，单主节点工作.
通过基于HTTP的pull方式采集时序数据
可以通过中间网关进行时序列数据推送(pushing)
目标服务器可以通过发现服务或者静态配置实现
多种可视化和仪表盘支持
        其中Prometheus生态系统可以有多个组件构成，大多组件都是独立工作的，可以有选择的配置自己需要的服务，主要有以下：

Prometheus 主服务,用来抓取和存储时序数据
client library 用来构造应用或 exporter 代码 (go,java,python,ruby)
push 网关可用来支持短连接任务
可视化的dashboard (两种选择,promdash 和 grafana.目前主流选择是 grafana.)
实验性的报警管理端(alertmanager,单独进行报警汇总,分发,屏蔽等 )

