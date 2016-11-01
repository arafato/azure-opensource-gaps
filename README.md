# Azure Opensource Gaps
A curated list of OSS projects that lack or have incomplete support for the Microsoft Azure platform.
A gap can be in one of the three states: **[OPEN]**, **[IN-PROGRESS]**, **[CLOSED]**.

## Apache Flink
Apache Flink is a community-driven open source framework for distributed big data analytics, like Hadoop and Spark. 
The core of Apache Flink is a distributed streaming dataflow engine written in Java and Scala.
It aims to bridge the gap between MapReduce-like systems and shared-nothing parallel database systems. 

- **[OPEN]** The official project repository does not provide a streaming connector for Azure Eventhub. 
The current list of streaming connectors can be found here:
[https://github.com/apache/flink/tree/master/flink-streaming-connectors](https://github.com/apache/flink/tree/master/flink-streaming-connectors)

## Terraform
Terraform provides a common configuration to launch infrastructure — from physical and virtual servers to email and DNS providers. 
Once launched, Terraform safely and efficiently changes infrastructure as the configuration is evolved.

- **[IN-PROGRESS]** Terraform lacks support of support for different Azure Environments such as GermanCloud, GovCloud, ChinaCloud.
PR at [https://github.com/hashicorp/terraform/issues/9400](https://github.com/hashicorp/terraform/issues/9400)

## SimpleKV
simplekv is an API for very basic key-value stores used for small, frequently accessed data or large binary blobs. It is written in Python.

- **[IN-PROGRESS]** SimpleKV lacks support of Azure Blob Storage.
PR at [https://github.com/mbr/simplekv/pull/35](https://github.com/mbr/simplekv/pull/35)