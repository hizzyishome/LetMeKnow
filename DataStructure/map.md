### Map

- HashMap  
最常用的Map,它根据键的HashCode 值存储数据,根据键可以直接获取它的值，具有很快的访问速度。HashMap最多只允许一条记录的键为Null(多条会覆盖);
允许多条记录的值为 Null。非同步的。

- TreeMap
能够把它保存的记录根据键(key)排序,默认是按升序排序，也可以指定排序的比较器，当用Iterator 遍历TreeMap时，得到的记录是排过序的。
TreeMap不允许key的值为null。非同步的。 

- Hashtable  
与HashMap类似,不同的是:key和value的值均不允许为null;它支持线程的同步，即任一时刻只有一个线程能写Hashtable,
因此也导致了Hashtale在写入时会比较慢。 

- LinkedHashMap  
保存了记录的插入顺序，在用Iterator遍历LinkedHashMap时，先得到的记录肯定是先插入的.在遍历的时候会比HashMap慢。
key和value均允许为空，非同步的。 

- 增强for循环使用方便，但性能较差，不适合处理超大量级的数据。

- 迭代器的遍历速度要比增强for循环快很多，是增强for循环的2倍左右。

- 使用entrySet遍历的速度要比keySet快很多，是keySet的1.5倍左右。