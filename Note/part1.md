#### 做一个简单的Read-Execute-Print-Loop

- main()函数要完成的是

  > - 无限的死循环
  > - 打印提示
  > - 得到输入行
  > - 处理输入行

- InputBuffer是作为一个warpper来存储当前的状态从而可以跟getline()进行交互的

- print_prompt()函数

  > - 打印提示给user
  > - 在读取每一个输入行之前

- getline()

  > - 读取输入行

- close_input_buffer()

  > - 释放实例InputBuffer*和实例buffer的内存

- 最后解析和执行command



---



#### [strcmp和strncmp](https://blog.csdn.net/qq_26093511/article/details/68483348)

#### [ssize_t和size_t](https://blog.csdn.net/bzhxuexi/article/details/19899803)

#### [typedef struct](https://blog.csdn.net/CHENYUFENG1991/article/details/50681497)