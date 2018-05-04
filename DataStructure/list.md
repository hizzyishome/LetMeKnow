###List



#### ArraryList
查询很快，但是中间部分的插入和删除很慢
如果预先能知道或者估计所需数据项个数的，需要传入initialCapacity,因为如果使用无参的构造函数，会首先把EMPTY_ELEMENTDATA赋值给elementData
然后根据插入个数于当前数组size比较，不停调用Arrays.copyOf()方法，扩展数组大小,造成性能浪费

#### Vector
Vector就是ArrayList的线程安全版，它的方法前都加了synchronized锁，其他实现逻辑都相同。 
如果对线程安全要求不高的话，可以选择ArrayList，毕竟synchronized也很耗性能

#### LinkedList
还是一个双向链表 默认删除头节点 
1.是按顺序查找 
2.允许存储项为空 
3.允许多个存储项的值相等