+++
date = '2025-10-15T22:08:13+08:00'
draft = false
title = 'Vector'
+++



# vector底层实现

在底层实现上，其实就是单纯的动态数组<br>

## vector的类构成
包含了三个内容:
M_start 容器开始的指针
M_finish 容器结束的位置
M_end_of_storage 动态内存
## vector扩容的底层原理
这三个指针就能够计算得到vector的大小（目前的有效元素个数）
容量（capacity）：capacity()是end_of_storage - start
当size追上了容量大小，那么就说明要扩容了，vector就会申请比原来的vector要大若干倍数的内存（）

## vector的空间释放


## vector 的类方法
### 构造函数
无参构造：
没有申请动态内存<br>
性能优先
