## 个人面试过程中的准备，主要是笔记整理和资料整理
**Table of Contents**
  * [Python语言特性](#python语言特性)
      * [1. Python的函数参数传递](#1-python的函数参数传递)
      * [2. Python中的元类(metaclass)](#2-python中的元类metaclass)
      * [3. @staticmethod和@classmethod](#3-staticmethod和classmethod)
      * [4. 类变量和实例变量](#4-类变量和实例变量)
      * [5. Python自省](#5-python自省)
      * [6. 字典推导式](#6-字典推导式)
      * [7. Python中单下划线和双下划线](#7-python中单下划线和双下划线)
      * [8. 字符串格式化:\x和.format](#8-字符串格式化和format)
      * [9. 迭代器和生成器](#9-迭代器和生成器)
      * [10. *args and <code>**kwargs</code>](#10-args-and-kwargs)
      * [11. 面向切面编程AOP和装饰器](#11-面向切面编程aop和装饰器)
      * [12. 鸭子类型](#12-鸭子类型)
      * [13. Python中重载](#13-python中重载)
      * [14. 新式类和旧式类](#14-新式类和旧式类)
      * [15. __new__和<code>__init__</code>的区别](#15-__new__和__init__的区别)
      * [16. 单例模式](#16-单例模式)
         * [1. 使用__new__方法](#1-使用__new__方法)
         * [2. 共享属性](#2-共享属性)
         * [3. 装饰器版本](#3-装饰器版本)
         * [4. import方法](#4-import方法)
      * [17. Python中的作用域](#17-python中的作用域)
      * [18. GIL线程全局锁](#18-gil线程全局锁)
      * [19. 协程](#19-协程)
      * [20. 闭包](#20-闭包)
      * [21. lambda函数](#21-lambda函数)
      * [22. Python函数式编程](#22-python函数式编程)
      * [23. Python里的拷贝](#23-python里的拷贝)
      * [24. Python垃圾回收机制](#24-python垃圾回收机制)
         * [1. 引用计数](#1-引用计数)
         * [2. 标记-清除机制](#2-标记-清除机制)
         * [3. 分代技术](#3-分代技术)
      * [25. Python的List](#25-python的list)
      * [26. Python的is](#26-python的is)
      * [27. read,readline和readlines](#27-readreadline和readlines)
      * [28. Python2和3的区别](#28-python2和3的区别)
      * [29. super init](#29-super-init)
      * [30. range and xrange](#30-range-and-xrange)
      
  * [Python问答](#python问答)
      * [1. 到底什么是Python？你可以在回答中与其他技术进行对比](#1-python的函数参数传递)
      * [2. 什么是PEP8？](#2-python中的元类metaclass)
      * [3. 什么是pickling和unpickling？](#3-staticmethod和classmethod)
      * [4. 说说python程序运行过程？](#4-类变量和实例变量)
      * [5. Python是怎样管理内存的？](#5-python自省)
      * [6. 流重定向](#6-字典推导式)
      * [7. python为什么不能像C++一样快?如果要追求速度该怎么做？](#7-python中单下划线和双下划线)
      * [8. 数组和元组之间的区别是什么？](#8-字符串格式化和format)
      * [9. 谈谈你对python中变量、对象和引用的理解](#9-迭代器和生成器)
      * [10. python中的冻结二进制文件你了解多少？](#10-args-and-kwargs)
      * [11. Python都有哪些自带的数据类型？](#11-面向切面编程aop和装饰器)
      * [12. 什么是Python的命名空间？](#12-鸭子类型)
      * [13. Python中的pass是什么？](#13-python中重载)
      * [14. 在Python中什么是slicing？](#14-新式类和旧式类)
      * [15. Python中的docstring是什么？](#15-__new__和__init__的区别)
      * [16. 如何在Python中拷贝一个对象？这些拷贝之间有什么区别？](#16-单例模式)
      * [17. Python中的负索引是什么？](#17-python中的作用域)
      * [18. 如何将一个数字转换成一个字符串？](#18-gil线程全局锁)
      * [19. Python中的模块和包是什么？](#19-协程)
      * [20. 函数中*args，**kwargs这两个参数是什么意思？我们为什么要使用它们？](#20-闭包)
      * [21. 谈一谈Python的装饰器（decorator）](#21-lambda函数)
      * [22. 简要描述Python的垃圾回收机制（garbage collection）](#22-python函数式编程)
      * [23. 说明os,sys模块不同，并列举常用的模块方法？](#23-python里的拷贝)
      * [24. 什么是lambda表达式？它有什么好处？](#24-python垃圾回收机制)
      * [25. 表达式与语句有什么区别？](#25-python的list)
      * [26. __new__和__init__的区别](#26-python的is)
      * [27. Python中单下划线和双下划线分别是什么？](#27-readreadline和readlines)
      * [28. 说一说Python自省](#28-python2和3的区别)
      * [29. 如何在一个函数内部修改全局变量](#29-super-init)
      * [30. 列出你知道的python标准库](#30-range-and-xrange)
      * [31. 如何删除字典的键以及如何合并两个字典](#21-lambda函数)
      * [32. python2和python3的range(100)的区别](#22-python函数式编程)
      * [33. 简述with方法打开处理文件帮我我们做了什么？](#23-python里的拷贝)
      * [34. 列表[1,2,3,4,5],请使用map()函数输出[1,4,9,16,25]，并使用列表推导式提取出大于10的数，最终输出[16,25]](#24-python垃圾回收机制)
      * [35. python中生成随机整数、随机小数、0-1之间小数方法](#25-python的list)
      * [36. python中的断言](#26-python的is)
      * [37. python2和python3区别？至少5个](#27-readreadline和readlines)
      * [38. 列出python中可变数据类型和不可变数据类型，并简述原理](#28-python2和3的区别)
      * [39. 字典根据键从小到大排序](#29-super-init)
      * [40. 过滤掉列表 a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]中的所有偶数](#30-range-and-xrange)
      * [41. 正则表达式匹配中，（.*）和（.*?）匹配区别？](#21-lambda函数)
      * [42. [[1,2],[3,4],[5,6]],一行代码展开该列表，得出[1,2,3,4,5,6]](#22-python函数式编程)
      * [43. 举例说明zip()函数用法](#23-python里的拷贝)
      * [44. 提高python运行效率的方法](#24-python垃圾回收机制)
      * [45. 如何四舍五入？](#25-python的list)
      * [46. 简述多线程、多进程](#26-python的is)
      * [47. 简述any()和all()方法](#27-readreadline和readlines)
      * [48. python中什么元素为假？](#28-python2和3的区别)
      * [49. IOError、AttributeError、ImportError、IndentationError、IndexError、KeyError、SyntaxError、NameError分别代表什么异常?](#29-super-init)
      * [50. sort()和sorted()有什么区别？](#30-range-and-xrange)
      * [51. lambda函数配合sorted()进行复杂排序](#21-lambda函数)
      * [52. 用两种方法去空格](#22-python函数式编程)
      * [53. 简述python引用计数机制](#23-python里的拷贝)
      * [54. Python传参数是传值还是传址？](#24-python垃圾回收机制)
      * [55. Python多线程（multi-threading）是个好主意吗？](#25-python的list)
      * [56. 异常模块中try except else finally的区别](#26-python的is)
      * [57. is与==有什么区别?](#27-readreadline和readlines)
      * [58. python除法‘/’ 与 ‘//’](#28-python2和3的区别)
      * [59. 集合有哪些运算?](#29-super-init)
      * [60. 列出字符串常用操作](#30-range-and-xrange)
      * [61. 列出列表的常用操作](#21-lambda函数)
      * [62. 两个等长列表如何构造字典？](#22-python函数式编程)
      * [63. 只有一个列表如何用enumerate构造字典？](#23-python里的拷贝)
      * [64. 迭代器和可迭代对象分别是什么，它们之间有什么区别？](#24-python垃圾回收机制)
      * [65. 单遍迭代器与多遍迭代器有什么区别？](#25-python的list)
      * [66. 什么是多态？](#26-python的is)
      * [67. 如何理解闭包？](#27-readreadline和readlines)
      * [68. 谈谈类中的访问限制](#28-python2和3的区别)
      
      
  * [编程题](#编程题)
      * [1. 台阶问题/斐波那契](#1-台阶问题斐波那契)
      * [2. 变态台阶问题](#2-变态台阶问题)
      * [3. 矩形覆盖](#3-矩形覆盖)
      * [4. 杨氏矩阵查找](#4-杨氏矩阵查找)
      * [5. 去除列表中的重复元素](#5-去除列表中的重复元素)
      * [6. 链表成对调换](#6-链表成对调换)
      * [7. 创建字典的方法](#7-创建字典的方法)
         * [1. 直接创建](#1-直接创建)
         * [2. 工厂方法](#2-工厂方法)
         * [3. fromkeys()方法](#3-fromkeys方法)
      * [8. 合并两个有序列表](#8-合并两个有序列表)
      * [9. 交叉链表求交点](#9-交叉链表求交点)
      * [10. 二分查找](#10-二分查找)
      * [11. 快排](#11-快排)
      * [12. 找零问题](#12-找零问题)
      * [13. 广度遍历和深度遍历二叉树](#13-广度遍历和深度遍历二叉树)
      * [14. 二叉树节点](#14-二叉树节点)
      * [15. 层次遍历](#15-层次遍历)
      * [16. 深度遍历](#16-深度遍历)
      * [17. 前中后序遍历](#17-前中后序遍历)
      * [18. 求最大树深](#18-求最大树深)
      * [19. 求两棵树是否相同](#19-求两棵树是否相同)
      * [20. 前序中序求后序](#20-前序中序求后序)
      * [21. 单链表逆置](#21-单链表逆置)
      * [22. 两个字符串是否是变位词](#22-两个字符串是否是变位词)
      * [23. 动态规划问题](#23-动态规划问题)
