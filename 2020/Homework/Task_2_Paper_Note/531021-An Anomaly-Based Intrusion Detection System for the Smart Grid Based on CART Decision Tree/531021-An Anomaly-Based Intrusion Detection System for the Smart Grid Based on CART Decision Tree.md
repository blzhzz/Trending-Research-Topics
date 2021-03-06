## "An Anomaly-Based Intrusion Detection System for the Smart Grid Based on CART Decision Tree" 论文笔记

**论文题目**：An Anomaly-Based Intrusion Detection System for the Smart Grid Based on CART Decision Tree

**论文作者**：Panagiotis I. Radoglou-Grammatikis ，Panagiotis G. Sarigiannidis

**论文出处**：IEEE， Global Information Infrastructure and Networking Symposium 

**笔记作者**：Matchtheworld

[原文链接](https://ieeexplore.ieee.org/document/8635743/)

### 论文笔记信息

---

#### 1. 研究背景

​	智能电网（SG）范式构成了常规电网的新一代，通过信息和通信技术（ICT）服务对其运行进行监控。根据，SG可能会构成物联网（IoT）（称为Enernet）的最大应用。特别是，SG提供的通信体系结构可增强能源的产生，传输和分配过程，从而为消费者和公司带来多种好处。SG结合了一组异构技术，例如智能电表，监控和数据采集（SCADA）系统，电动汽车，自动化变电站和同步相量系统。这些技术中的每一种都以各种安全威胁为特征，这些安全威胁可能导致毁灭性后果，例如断电和掉电。在SG中，网络攻击通常首先针对计算系统的可用性和完整性，而其次针对机密性。例如，各种拒绝服务（DoS）和分布式DoS（DDoS）攻击可能会损害系统的可用性。另一方面，虚假数据注入（FDI）攻击会危害信息的完整性。最后，中间人（MiTM）攻击可能威胁系统的机密性。在这篇论文中，作者提出了用于高级计量基础架构（AMI）的IDS，该IDS利用决策树来检测可能的网络攻击。

#### 2. 主要内容

​	将IDS集中部署在AMI体系结构的数据收集器设备发送和接收的网络流上。因为这些设备是AMI的最关键组件，同时它构成了消费者和公司之间连接的中间点。它可以同时接收智能电表和AMI前端的数据。因此数据收集器设备的安全性对于SG的整体保护至关重要。基于捕获的网络流、基于异常的IDS可以将其分类为正常行为或可能的网络攻击。文中的IDS的体系结构包含四个模块：

- **网络监控模块**：网络监视模块负责监视和捕获在数据收集器和其他设备之间交换的传输控制协议通信。
- **网络流提取模块**：网络流提取模块从前一个模块接收网络流量，并提取相应的双向网络流。
- **分析引擎模块**：分析引擎模块构成了提议的IDS的核心，并负责检测可能的网络攻击。该模块利用决策树从先前的模块接收网络流的选定特征。
- **响应模块**：响应模块执行提议的IDS的最后过程，它将可能的网络攻击通知系统或安全管理员。

#### 3. 创新点

- 利用机器学习来增强基于异常的智能电网入侵检测系统的能力，利用决策树模型来检测可能的网络攻击。
- 基于异常的IDS 能够检测到未知的网络攻击方式。

#### 4. 论文缺点

- 采用的数据集比较的老，不是具有明显的普遍性和跨库。
- 采用的是集中式的统一入侵检测。

#### 5 论文可以改进的地方

- 在实际的场景中去创建新的数据集用于本文提出的系统的测试，同时对模型进行进一步的优化。
- 可以采用分布式异常的IDS系统来监视和控制AMI所有组件的网络活动。系统将由单独的IDS代理组成，这些代理将监视智能电表，数据收集器和AMI前端的网络活动。



