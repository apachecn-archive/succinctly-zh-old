## 摘要

在本章中，我们研究了 HBase 中表设计的关键部分：构造行键，预分割区域以及使用列和列族。

没有一种设计适合所有 HBase 问题;您需要了解性能和使用注意事项，尤其是行键设计。您需要根据所期望的访问模式设计表，并且在开发过程中重新设计表并不常见，因为您可以了解有关需求的更多信息。

现在我们对 HBase 如何存储数据有很好的工作知识;在接下来的几章中，我们将使用 HBase 提供的 API 提供远程访问数据：Java，Thrift 和 REST。