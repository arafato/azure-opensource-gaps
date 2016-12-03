# Azure Opensource Gaps
A curated list of OSS projects that lack or have incomplete support for the Microsoft Azure platform.
A gap can be in one of the three states: **[OPEN]**, **[IN-PROGRESS]**, **[CLOSED]**.

## Apache Flink
[Apache Flink](https://flink.apache.org/) is a community-driven open source framework for distributed big data analytics, like Hadoop and Spark. 
The core of Apache Flink is a distributed streaming dataflow engine written in Java and Scala.
It aims to bridge the gap between MapReduce-like systems and shared-nothing parallel database systems. 
- **[OPEN]** The official project repository does not provide a streaming connector for Azure Eventhub. 
The current list of streaming connectors can be found here:
[https://github.com/apache/flink/tree/master/flink-streaming-connectors](https://github.com/apache/flink/tree/master/flink-streaming-connectors)

## Cross-Platform Azure Storage Emulator
Currently, there only exists a Windows-only Azure Storage Emulator.
- **[IN-PROGRESS]** [Azurit](https://github.com/arafato/azurite) is a lightweight and cross-platform server clone
of Azure Blob Storage that simulates most of the commands supported by it with minimal dependencies.

## Serverless Framework
The framework uses new event-driven compute services, like AWS Lambda, Google CloudFunctions, and more. It's a command-line tool, 
providing scaffolding, workflow automation and best practices for developing and deploying your serverless architecture. 
It's also completely extensible via plugins.

- **[IN-PROGRESS]** Azure support is actively being worked on based on a first [PR](https://github.com/serverless/serverless/pull/1426) 
by the Microsoft Open Source Team. Current tracking item is here: [https://github.com/serverless/serverless/issues/1493](https://github.com/serverless/serverless/issues/1493)

## Terraform
[Terraform](https://www.terraform.io/) provides a common configuration to launch infrastructure — from physical and virtual servers to email and DNS providers. 
Once launched, Terraform safely and efficiently changes infrastructure as the configuration is evolved.

- **[CLOSED]** Terraform lacks support for different Azure Environments such as GermanCloud, GovCloud, ChinaCloud.
PR at [https://github.com/hashicorp/terraform/issues/9400](https://github.com/hashicorp/terraform/issues/9400)

## SimpleKV
[SimpleKV](https://github.com/mbr/simplekv) is an API for very basic key-value stores used for small, frequently accessed data or large binary blobs. It is written in Python.

- **[IN-PROGRESS]** SimpleKV lacks support of Azure Blob Storage.
PR at [https://github.com/mbr/simplekv/pull/35](https://github.com/mbr/simplekv/pull/35)