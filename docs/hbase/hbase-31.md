## 摘要

Java API 是 HBase 最丰富的客户端接口，除此之外还有许多其他功能，包括递增计数器列，访问随机数据项的功能（对集成测试很有用）以及一组管理操作。

Java 访问直接指向区域服务器（或管理功能的主服务器），它是最有效的 API。它不需要在区域服务器上运行任何其他 JVM，并且客户端可以识别区域，因此它直接从托管该区域的服务器请求数据。

Java 也是在服务器上扩展 HBase 的本机语言。协处理器是一个高级主题，我不会在本书中介绍，但它们在许多场景中都很有价值。您使用 Java 编写协处理器，并将该程序包提供给 HDFS 上的 Region Servers。然后可以在服务器上调用您的代码以响应数据操作，例如添加行或更改单元格值时，类似于 SQL 数据库中的触发器。

即使您只使用 Java 工作，也很了解外部 HBase API 提供的内容及其工作原理。在下一章中，我们将介绍 Thrift API，它与 Java 功能集几乎相同，并且可以从许多客户端库中使用。我们将介绍如何使用 Thrift 和 Python。