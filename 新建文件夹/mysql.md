



![1646707547829](C:\Users\ADMINI~1\AppData\Local\Temp\1646707547829.png)



命令行



![1646707702305](C:\Users\ADMINI~1\AppData\Local\Temp\1646707702305.png)







# 数据库引擎

![1646708211429](C:\Users\ADMINI~1\AppData\Local\Temp\1646708211429.png)

![1646708389341](C:\Users\ADMINI~1\AppData\Local\Temp\1646708389341.png)

# 设置字符集编码

![1646708599265](C:\Users\ADMINI~1\AppData\Local\Temp\1646708599265.png)



# 表、字段的操作（修改、删除）

## 修改

![1646708943862](C:\Users\ADMINI~1\AppData\Local\Temp\1646708943862.png)

区别：modify只能修改约束；change修改字段命，但可以在修改约束。

![1646709047183](C:\Users\ADMINI~1\AppData\Local\Temp\1646709047183.png)



## 删除

![1646709225441](C:\Users\ADMINI~1\AppData\Local\Temp\1646709225441.png)

## 注意

![1646709250585](C:\Users\ADMINI~1\AppData\Local\Temp\1646709250585.png)



# 常用函数

![1646710869017](C:\Users\ADMINI~1\AppData\Local\Temp\1646710869017.png)



![1646711145992](C:\Users\ADMINI~1\AppData\Local\Temp\1646711145992.png)



![1646711213957](C:\Users\ADMINI~1\AppData\Local\Temp\1646711213957.png)



# 聚合函数

![1646711479961](C:\Users\ADMINI~1\AppData\Local\Temp\1646711479961.png)



# 分组和过滤

分组 ：GROUP BY

过滤：后面应该用having代替where

![1646711666663](C:\Users\ADMINI~1\AppData\Local\Temp\1646711666663.png)



# 关键词顺序

![1646711815172](C:\Users\ADMINI~1\AppData\Local\Temp\1646711815172.png)



# 分页和排序

![1646711926815](C:\Users\ADMINI~1\AppData\Local\Temp\1646711926815.png)



![1646712256747](C:\Users\ADMINI~1\AppData\Local\Temp\1646712256747.png)

![1646712233493](C:\Users\ADMINI~1\AppData\Local\Temp\1646712233493.png)





# mysql优化

![1647400073606](C:\Users\ADMINI~1\AppData\Local\Temp\1647400073606.png)

![1647400531631](C:\Users\ADMINI~1\AppData\Local\Temp\1647400531631.png)

![1647400506602](C:\Users\ADMINI~1\AppData\Local\Temp\1647400506602.png)



![1647400551417](C:\Users\ADMINI~1\AppData\Local\Temp\1647400551417.png)



数据库面试题

https://blog.csdn.net/qq_22222499/article/details/79060495



# 为什么使用B+Tree

索引查找过程中就要产生磁盘I/O消耗,主要看IO次数，和磁盘存取原理有关。
根据B-Tree的定义，可知检索一次最多需要访问h个节点。数据库系统的设计者巧妙利用了磁盘预读原理，
将一个节点的大小设为等于一个页，这样每个节点只需要一次I/O就可以完全载入
局部性原理与磁盘预读



# 数据库三范式

| 级别 | 概念                                                         |
| ---- | ------------------------------------------------------------ |
| 1NF  | 属性不可分（**列不可再分**）                                 |
| 2NF  | 非主键属性，完全依赖于主键属性 **(确保表中的每列都和主键相关)** |
| 3NF  | 非主键属性无传递依赖                                         |