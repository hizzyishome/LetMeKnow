### Set
***无序,不能重复***

#### HashSet
线程不安全，存取速度快。底层是以hash表实现的。
对象的相等性:引用到堆上同一个对象的两个引用是相等的。如果对两个引用调用hashCode方法，会得到相同的结果.
如果对象所属的类没有覆盖Object的hashCode方法的话，hashCode会返回每个对象特有的序号（java是依据对象的内存地址计算出的此序号），
所以两个不同的对象的hashCode值是不可能相等的。

hashcode -> 如果哈希值一样 -> equals方法 -> true -> 视为同一个元素
哈希值相同equals为false -> 在同样的哈希值下顺延 -> 哈希值相同的元素放在一个哈希桶中
一个hashCode位置上可以存放多个元素

#### TreeSet
不能重复存储元素，而且要排序 
红黑树是一种特定类型的二叉树
红黑树算法的规则: 左小右大。
元素自身 需要元素实现Comparable接口，重写compareTo方法
容器 接口Comparator，重写compare方法(同时存在，为主)

##### LinkedHashSet
会保存插入的顺序

看到array，就要想到角标。

看到link，就要想到first，last。

看到hash，就要想到hashCode,equals.

看到tree，就要想到两个接口。Comparable，Comparator。

