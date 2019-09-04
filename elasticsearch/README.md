## Elasticsearch

1. 基础概念
    - Document：表的行
    - Index：表
    - Node：ES的一个运行实例
    - Cluster：由一个或多个节点组成，对外提供服务
    - 文档id：行主键
 
 2. 数据类型
    - 字符串：text(分词)，keyword(不分词)
    - 数值型： long, integer, short, byte, double, float, half_float, scaled_float
    - 布尔：boolean
    - 日期： date
    - 二进制： binary
    - 范围类型： integer_range, float_range, long_range, double_range, date_range
 
 3. 元数据
    - _index: 文档索引名
    - _type: 文档类型名
    - _id: 文档唯一id
    - _uid: 组合id，由_type和_id组成（由于_type废弃，所以同_id一样）
    - _source: 文档原始json数据
    - _all: 整合所有字段内容到该字段，默认禁用