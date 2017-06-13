#统一监控平台
---
任何一种架构选择都必然有利有弊。特别是在面向服务的分布式架构方面，相对于单一且经过严格定义的大规模开发项目，分布式架构要求大家面对由众多小型服务所构成的复杂生态系统。尤其是在出现生产问题、异常或BUG的时候，如何做到快速报警、定位问题、快速解决都是分布式架构必须面临的问题。基于此，我们在进行新一代交易系统建设的同时，也进行了统一监控平台的建设。
统一监控平台的整体架构图，如下图所示：

- 1、统一监控平台基于开源ELK架构构件，同时基于数据交换平台和各分布式节点上的服务进行通讯，采集监控信息。
- 2、统一监控平台采用基于Groovy的脚本语言对于监控规则进行定制，具有强大的可扩展能力。
- 3、统一监控平台利用ElasticSeach的强大日志信息聚合分析能力，对于大数据日志文件进行分析，并实时报警。
- 4、基于统一监控平台我们建立了标准的日志跟踪规范，用于跟踪关键数据流的流向，以便于进行性能、异常情况的分析。

通过建设统一监控平台，将现有的应用监控提升到业务和技术两方面的视角，将业务运行健康情况和技术监控指标集中展示和监控，有助于提前预警、快速定位和解决问题，为保障生产系统安全运行、提高主动式运维水平提供技术支撑。	
 
