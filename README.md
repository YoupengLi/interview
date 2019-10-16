## 个人面试过程中的准备，主要是笔记整理和资料整理
**Table of Contents**
  * [Python语言特性](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md)
      * [1. Python的函数参数传递](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#1-python的函数参数传递)
      * [2. Python中的元类(metaclass)](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#2-python中的元类metaclass)
      * [3. @staticmethod和@classmethod](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#3-staticmethod和classmethod)
      * [4. 类变量和实例变量](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#4-类变量和实例变量)
      * [5. Python自省](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#5-python自省)
      * [6. 字典推导式](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#6-字典推导式)
      * [7. Python中单下划线和双下划线](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#7-python中单下划线和双下划线)
      * [8. 字符串格式化:\x和.format](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#8-字符串格式化和format)
      * [9. 迭代器和生成器](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#9-迭代器和生成器)
      * [10. *args and <code>**kwargs</code>](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#10-args-and-kwargs)
      * [11. 面向切面编程AOP和装饰器](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#11-面向切面编程aop和装饰器)
      * [12. 鸭子类型](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#12-鸭子类型)
      * [13. Python中重载](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#13-python中重载)
      * [14. 新式类和旧式类](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#14-新式类和旧式类)
      * [15. __new__和<code>__init__</code>的区别](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#15-__new__和__init__的区别)
      * [16. 单例模式](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#16-单例模式)
         * [1. 使用__new__方法](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#1-使用__new__方法)
         * [2. 共享属性](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#2-共享属性)
         * [3. 装饰器版本](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#3-装饰器版本)
         * [4. import方法](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#4-import方法)
      * [17. Python中的作用域](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#17-python中的作用域)
      * [18. GIL线程全局锁](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#18-gil线程全局锁)
      * [19. 协程](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#19-协程)
      * [20. 闭包](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#20-闭包)
      * [21. lambda函数](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#21-lambda函数)
      * [22. Python函数式编程](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#22-python函数式编程)
      * [23. Python里的拷贝](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#23-python里的拷贝)
      * [24. Python垃圾回收机制](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#24-python垃圾回收机制)
         * [1. 引用计数](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#1-引用计数)
         * [2. 标记-清除机制](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#2-标记-清除机制)
         * [3. 分代技术](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#3-分代技术)
      * [25. Python的List](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#25-python的list)
      * [26. Python的is](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#26-python的is)
      * [27. read,readline和readlines](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#27-readreadline和readlines)
      * [28. Python2和3的区别](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#28-python2和3的区别)
      * [29. super init](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#29-super-init)
      * [30. range and xrange](https://github.com/YoupengLi/interview/blob/master/Python语言特性.md#30-range-and-xrange)
      
  * [Python问答](https://github.com/YoupengLi/interview/blob/master/Python问答.md)
      * [1. 到底什么是Python？你可以在回答中与其他技术进行对比](https://github.com/YoupengLi/interview/blob/master/Python问答.md#1-到底什么是Python你可以在回答中与其他技术进行对比)
      * [2. 什么是PEP8？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#2-什么是pep8)
      * [3. 什么是pickling和unpickling？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#3-什么是pickling和unpickling)
      * [4. 说说Python程序运行过程？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#4-说说python程序运行过程)
      * [5. Python是怎样管理内存的？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#5-python是怎样管理内存的)
      * [6. 流重定向](https://github.com/YoupengLi/interview/blob/master/Python问答.md#6-流重定向)
      * [7. Python为什么不能像C++一样快？如果要追求速度该怎么做？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#7-python为什么不能像c一样快如果要追求速度该怎么做)
      * [8. 数组和元组之间的区别是什么？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#8-数组和元组之间的区别是什么)
      * [9. 谈谈你对Python中变量、对象和引用的理解](https://github.com/YoupengLi/interview/blob/master/Python问答.md#9-谈谈你对python中变量对象和引用的理解)
      * [10. Python中的冻结二进制文件你了解多少？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#10-python中的冻结二进制文件你了解多少)
      * [11. Python都有哪些自带的数据类型？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#11-python都有哪些自带的数据类型)
      * [12. 什么是Python的命名空间？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#12-什么是python的命名空间)
      * [13. Python中的pass是什么？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#13-python中的pass是什么)
      * [14. 在Python中什么是slicing？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#14-在python中什么是slicing)
      * [15. Python中的docstring是什么？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#15-python中的docstring是什么)
      * [16. 如何在Python中拷贝一个对象？这些拷贝之间有什么区别？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#16-如何在python中拷贝一个对象这些拷贝之间有什么区别)
      * [17. Python中的负索引是什么？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#17-python中的负索引是什么)
      * [18. 如何将一个数字转换成一个字符串？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#18-如何将一个数字转换成一个字符串)
      * [19. Python中的模块和包是什么？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#19-python中的模块和包是什么)
      * [20. 函数中*args、**kwargs这两个参数是什么意思？我们为什么要使用它们？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#20-函数中argskwargs这两个参数是什么意思我们为什么要使用它们)
      * [21. 谈一谈Python的装饰器（decorator）](https://github.com/YoupengLi/interview/blob/master/Python问答.md#21-谈一谈python的装饰器decorator)
      * [22. 简要描述Python的垃圾回收机制（garbage collection）](https://github.com/YoupengLi/interview/blob/master/Python问答.md#22-简要描述python的垃圾回收机制garbage-collection)
      * [23. 说明os、sys模块不同，并列举常用的模块方法？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#23-说明ossys模块不同并列举常用的模块方法)
      * [24. 什么是lambda表达式？它有什么好处？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#24-什么是lambda表达式它有什么好处)
      * [25. 表达式与语句有什么区别？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#25-表达式与语句有什么区别)
      * [26. __new__和__init__的区别](https://github.com/YoupengLi/interview/blob/master/Python问答.md#26-__new__和__init__的区别)
      * [27. Python中单下划线和双下划线分别是什么？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#27-python中单下划线和双下划线分别是什么)
      * [28. 说一说Python自省](https://github.com/YoupengLi/interview/blob/master/Python问答.md#28-说一说python自省)
      * [29. 如何在一个函数内部修改全局变量](https://github.com/YoupengLi/interview/blob/master/Python问答.md#29-如何在一个函数内部修改全局变量)
      * [30. 列出你知道的Python标准库](https://github.com/YoupengLi/interview/blob/master/Python问答.md#30-列出你知道的python标准库)
      * [31. 如何删除字典的键以及如何合并两个字典](https://github.com/YoupengLi/interview/blob/master/Python问答.md#31-如何删除字典的键以及如何合并两个字典)
      * [32. Python2和Python3的range(100)的区别](https://github.com/YoupengLi/interview/blob/master/Python问答.md#32-python2和python3的range100的区别)
      * [33. 简述with方法打开处理文件帮我我们做了什么？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#33-简述with方法打开处理文件帮我我们做了什么)
      * [34. 列表[1,2,3,4,5],请使用map()函数输出[1,4,9,16,25]，并使用列表推导式提取出大于10的数，最终输出[16,25]](https://github.com/YoupengLi/interview/blob/master/Python问答.md#34-列表12345请使用map函数输出1491625并使用列表推导式提取出大于10的数，最终输出1625)
      * [35. Python中生成随机整数、随机小数、0-1之间小数方法](https://github.com/YoupengLi/interview/blob/master/Python问答.md#35-python中生成随机整数随机小数0-1之间小数方法)
      * [36. Python中的断言](https://github.com/YoupengLi/interview/blob/master/Python问答.md#36-python中的断言)
      * [37. Python2和Python3区别？至少5个](https://github.com/YoupengLi/interview/blob/master/Python问答.md#37-python2和python3区别至少5个)
      * [38. 列出Python中可变数据类型和不可变数据类型，并简述原理](https://github.com/YoupengLi/interview/blob/master/Python问答.md#38-列出python中可变数据类型和不可变数据类型并简述原理)
      * [39. 字典根据键从小到大排序](https://github.com/YoupengLi/interview/blob/master/Python问答.md#39-字典根据键从小到大排序)
      * [40. 过滤掉列表 a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]中的所有偶数](https://github.com/YoupengLi/interview/blob/master/Python问答.md#40-过滤掉列表a--1-2-3-4-5-6-7-8-9-10中的所有偶数)
      * [41. 正则表达式匹配中，（.*）和（.*?）匹配区别？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#41-正则表达式匹配中和匹配区别)
      * [42. [[1,2],[3,4],[5,6]],一行代码展开该列表，得出[1,2,3,4,5,6]](https://github.com/YoupengLi/interview/blob/master/Python问答.md#42-123456一行代码展开该列表，得出123456)
      * [43. 举例说明zip()函数用法](https://github.com/YoupengLi/interview/blob/master/Python问答.md#43-举例说明zip函数用法)
      * [44. 提高Python运行效率的方法](https://github.com/YoupengLi/interview/blob/master/Python问答.md#44-提高python运行效率的方法)
      * [45. 如何四舍五入？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#45-如何四舍五入)
      * [46. 简述多线程、多进程](https://github.com/YoupengLi/interview/blob/master/Python问答.md#46-简述多线程多进程)
      * [47. 简述any()和all()方法](https://github.com/YoupengLi/interview/blob/master/Python问答.md#47-简述any和all方法)
      * [48. Python中什么元素为假？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#48-python中什么元素为假)
      * [49. IOError、AttributeError、ImportError、IndentationError、IndexError、KeyError、SyntaxError、NameError分别代表什么异常?](https://github.com/YoupengLi/interview/blob/master/Python问答.md#49-IOErrorAttributeErrorImportErrorIndentationErrorIndexErrorKeyErrorSyntaxErrorNameError分别代表什么异常)
      * [50. sort()和sorted()有什么区别？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#50-sort和sorted有什么区别)
      * [51. lambda函数配合sorted()进行复杂排序](https://github.com/YoupengLi/interview/blob/master/Python问答.md#51-lambda函数配合sorted进行复杂排序)
      * [52. 用两种方法去空格](https://github.com/YoupengLi/interview/blob/master/Python问答.md#52-用两种方法去空格)
      * [53. 简述Python引用计数机制](https://github.com/YoupengLi/interview/blob/master/Python问答.md#53-简述python引用计数机制)
      * [54. Python传参数是传值还是传址？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#54-python传参数是传值还是传址)
      * [55. Python多线程（multi-threading）是个好主意吗？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#55-python多线程multi-threading是个好主意吗)
      * [56. 异常模块中try except else finally的区别](https://github.com/YoupengLi/interview/blob/master/Python问答.md#56-异常模块中try-except-else-finally的区别)
      * [57. is与==有什么区别?](https://github.com/YoupengLi/interview/blob/master/Python问答.md#57-is与有什么区别)
      * [58. Python除法‘/’ 与 ‘//’](https://github.com/YoupengLi/interview/blob/master/Python问答.md#58-python除法-与-)
      * [59. 集合有哪些运算？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#59-集合有哪些运算)
      * [60. 列出字符串常用操作](https://github.com/YoupengLi/interview/blob/master/Python问答.md#60-列出字符串常用操作)
      * [61. 列出列表的常用操作](https://github.com/YoupengLi/interview/blob/master/Python问答.md#61-列出列表的常用操作)
      * [62. 两个等长列表如何构造字典？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#62-两个等长列表如何构造字典)
      * [63. 只有一个列表如何用enumerate构造字典？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#63-只有一个列表如何用enumerate构造字典)
      * [64. 迭代器和可迭代对象分别是什么，它们之间有什么区别？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#64-迭代器和可迭代对象分别是什么它们之间有什么区别)
      * [65. 单遍迭代器与多遍迭代器有什么区别？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#65-单遍迭代器与多遍迭代器有什么区别)
      * [66. 什么是多态？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#66-什么是多态)
      * [67. 如何理解闭包？](https://github.com/YoupengLi/interview/blob/master/Python问答.md#67-如何理解闭包)
      * [68. 谈谈类中的访问限制](https://github.com/YoupengLi/interview/blob/master/Python问答.md#68-谈谈类中的访问限制)
      
  * [编程题](https://github.com/YoupengLi/interview/blob/master/编程题.md)
      * [1. 台阶问题/斐波那契](https://github.com/YoupengLi/interview/blob/master/编程题.md#1-台阶问题斐波那契)
      * [2. 变态台阶问题](https://github.com/YoupengLi/interview/blob/master/编程题.md#2-变态台阶问题)
      * [3. 矩形覆盖](https://github.com/YoupengLi/interview/blob/master/编程题.md#3-矩形覆盖)
      * [4. 杨氏矩阵查找](https://github.com/YoupengLi/interview/blob/master/编程题.md#4-杨氏矩阵查找)
      * [5. 去除列表中的重复元素](https://github.com/YoupengLi/interview/blob/master/编程题.md#5-去除列表中的重复元素)
      * [6. 链表成对调换](https://github.com/YoupengLi/interview/blob/master/编程题.md#6-链表成对调换)
      * [7. 创建字典的方法](https://github.com/YoupengLi/interview/blob/master/编程题.md#7-创建字典的方法)
         * [1. 直接创建](https://github.com/YoupengLi/interview/blob/master/编程题.md#1-直接创建)
         * [2. 工厂方法](https://github.com/YoupengLi/interview/blob/master/编程题.md#2-工厂方法)
         * [3. fromkeys()方法](https://github.com/YoupengLi/interview/blob/master/编程题.md#3-fromkeys方法)
      * [8. 合并两个有序列表](https://github.com/YoupengLi/interview/blob/master/编程题.md#8-合并两个有序列表)
      * [9. 交叉链表求交点](https://github.com/YoupengLi/interview/blob/master/编程题.md#9-交叉链表求交点)
      * [10. 二分查找](https://github.com/YoupengLi/interview/blob/master/编程题.md#10-二分查找)
      * [11. 快排](https://github.com/YoupengLi/interview/blob/master/编程题.md#11-快排)
      * [12. 找零问题](https://github.com/YoupengLi/interview/blob/master/编程题.md#12-找零问题)
      * [13. 广度遍历和深度遍历二叉树](https://github.com/YoupengLi/interview/blob/master/编程题.md#13-广度遍历和深度遍历二叉树)
      * [14. 二叉树节点](https://github.com/YoupengLi/interview/blob/master/编程题.md#14-二叉树节点)
      * [15. 层次遍历](https://github.com/YoupengLi/interview/blob/master/编程题.md#15-层次遍历)
      * [16. 深度遍历](https://github.com/YoupengLi/interview/blob/master/编程题.md#16-深度遍历)
      * [17. 前中后序遍历](https://github.com/YoupengLi/interview/blob/master/编程题.md#17-前中后序遍历)
      * [18. 求最大树深](https://github.com/YoupengLi/interview/blob/master/编程题.md#18-求最大树深)
      * [19. 求两棵树是否相同](https://github.com/YoupengLi/interview/blob/master/编程题.md#19-求两棵树是否相同)
      * [20. 前序中序求后序](https://github.com/YoupengLi/interview/blob/master/编程题.md#20-前序中序求后序)
      * [21. 单链表逆置](https://github.com/YoupengLi/interview/blob/master/编程题.md#21-单链表逆置)
      * [22. 两个字符串是否是变位词](https://github.com/YoupengLi/interview/blob/master/编程题.md#22-两个字符串是否是变位词)
      * [23. 动态规划问题](https://github.com/YoupengLi/interview/blob/master/编程题.md#23-动态规划问题)
