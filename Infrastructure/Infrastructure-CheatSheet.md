[![返回目录](https://parg.co/UCb)](https://github.com/wx-chevalier/Awesome-CheatSheets)

# Infrastructure CheatSheet

2005 年亚马逊发布了 AWS，算是拉开了云计算的序幕。云计算最重要的技术是分布式计算和分布式存储，分布式计算方面，最开始的技术是虚拟化，也就是所谓的“Software defined xxx”，通过对计算 / 存储和网络资源的虚拟化，同时能够给用户任意分配资源。但这里面一开始做的最好的只有文件存储这一块，AWS S3 及类似的对象存储产品给人们带来了云时代的一些实际的体验，但云服务器则还是走回了卖服务器的老路。

在云计算的发展过程中，有一个分支是 PaaS，最早是 2007 年推出的 Heroku，从形态上来说，它是一个 App Engine，提供应用的运行环境。2014 年 AWS 推出 Lambda 服务，Serverless 开始成为热词，从理论上说，Serverless 可以做到 NoOps、自动扩容和按使用付费，也被视为云计算的未来。但是，Serverless 本身有一些问题，比如难以解决的冷启动性能问题。

虚拟化：将硬件资源虚拟为软件资源，然后进行统一调度和管理。
隔离：从虚拟机到容器，再到虚拟机与容器融合，隔离的技术定义了云的形态。
解耦：无论是后端的微服务、前端的前后端分离、组件化等等，都是将关注点分离，解耦合的过程。
编排：大量不同的服务、任务，让他们组成一个整体，相互间能良好的协作。
智能化：让服务个性化，或者让自动化替代以前需要人工完成的事情。
实时化：计算和处理在极短时间内完成，从而实时的给予反馈。

# 大数据与分布式处理

Google 在 03-06 年发布了关于 GFS、BigTable、MapReduce 的三篇论文，开启了大数据时代。在发展的早期，就诞生了以 HDFS/HBase/MapReduce 为主的 Hadoop 技术栈，并一直延续到今天。

最开始大数据的处理大多是离线处理，MapReduce 理念虽然好，但性能捉急，新出现的 Spark 抓住了这个机会，依靠其强大而高性能的批处理技术，顺利取代了 MapReduce，成为主流的大数据处理引擎。
随着时代的发展，实时处理的需求越来越多，虽然 Spark 推出了 Spark Streaming 以微批处理来模拟准实时的情况，但在延时上还是不尽如人意。2011 年，Twitter 的 Storm 吹响了真正流处理的号角，而 Flink 则将之发扬光大。
到现在，Flink 的目光也不再将自己仅仅视为流计算引擎，而是更为通用的处理引擎，开始正面挑战 Spark 的地位。
