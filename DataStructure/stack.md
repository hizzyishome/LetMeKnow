### Stack
后进先出 LIFO
栈是一种用于存储数据的简单数据结构，有点类似链表或者顺序表（统称线性表），栈与线性表的最大区别是
数据的存取的操作，我们可以这样认为栈(Stack)是一种特殊的线性表，其插入和删除操作只允许在线性表的一端进行，
一般而言，把允许操作的一端称为栈顶(Top)，不可操作的一端称为栈底(Bottom)，
同时把插入元素的操作称为入栈(Push),删除元素的操作称为出栈(Pop)。若栈中没有任何元素，则称为空栈

- 顺序栈
- 链式栈

由于都是对栈顶操作的，所以大部分操作都是常数时间内完成的
- 符号匹配

- 中缀表达式转换为后缀表达式
    1. 如果遇到操作数，我们就直接将其放入数组B中。 
    2. 如果遇到运算符，则我们将其放入到栈A中，遇到左括号时我们也将其放入栈A中。 
    3. 如果遇到一个右括号，则将栈元素弹出，将弹出的运算符输出并存入数组B中直到遇到左括号为止。注意，左括号只弹出并不存入数组。 
    4. 如果遇到任何其他的操作符，如（“+”， “*”，“（”）等，从栈中弹出元素存入数组B直到遇到发现更低优先级的元素(或者栈为空)为止。弹出完这些元素后，才将遇到的操作符压入到栈中。有一点需要注意，只有在遇到” ) “的情况下我们才弹出” ( “，其他情况我们都不会弹出” ( “。 
    5. 如果我们读到了输入的末尾，则将栈中所有元素依次弹出存入到数组B中。 
    6. 到此中缀表达式转化为后缀表达式完成，数组存储的元素顺序就代表转化后的后缀表达式。 
- 计算后缀表达式
    1. 如果ch是数字，先将其转换为整数再入栈 
    2. 如果是运算符，将两个操作数出栈，计算结果再入栈 
    3. 重复1和2直到后缀表达式结束，最终栈内的元素即为计算的结果。
- 实现函数的嵌套调用
- HTML和XML文件中的标签匹配
- 网页浏览器中已访问页面的历史记录