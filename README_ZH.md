# 数据迁移学习笔记

主要对两款目前国内主流的RDBMS: MySQL和TiDB向下游数据源同步数据的技术方案进行整理. 包括:

| Source | Sink |
|:---:|:---:|
| MySQL | TiDB |
| MySQL | ClickHouse |
| MySQL | Doris |
| TiDB | TiDB |
| TiDB | ClickHouse |
| TiDB | Doris |

对每一组Source-Sink, 如果存在多种可行的同步方案, 也会尽量全部进行调研测试并给出优缺点.

数据同步要求:

- 全量同步
- 增量同步
- DDL同步
- 数据校验
