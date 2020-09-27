- SQLlite的前端是一个SQL编译器

  > - 这个compiler可以解析字符串并输出一个叫做**字节码**的内部表达式
  > - `prepare_statement()`函数就是我们的SQL编译器

- SQL编译器输出的字节码会被传输到虚拟机

  > - 虚拟机来执行接收到的字节码（代码中的`statement`）
  > - `execute_statement()`函数就是我们的虚拟机

- 虚拟机不用考虑syntax errors

- 允许一次编译多个**常用查询**并缓存字节码可以improved performance

- 编译器`prepare_statement`可以将**输入行**转换为**语句的内部表达式**，这就是我们SQLlite的前端。

- do_meta_command()是为了简洁

- 对于`insert()`函数使用了`strncmp()`函数，因为`insert`命令后面还会跟一些字符串，比如`insert foo bar`，所以使用strncmp而不是strcmp。

- typedef enum的作用就是定义一个类型。



### ---



#### [enum](https://www.runoob.com/cprogramming/c-enum.html)

#### [typedef enum](https://www.cnblogs.com/jcsu/articles/1299051.html)

#### [strncmp()函数](http://c.biancheng.net/cpp/html/2717.html)