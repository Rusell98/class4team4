# **关于“使用c++解决数独问题”的Code Review**
## 一、代码格式方面
代码的格式基本符合要求，表达较为清晰，没有明显逻辑与格式的错误。

---
## 二、代码可读性方面
1. 代码缺少注释，应在每个函数以及重要变量前面加入以“//”开头的注释，方便理解程序，同时也方便作者日后改进程序。
2. 代码中部分变量命名不够标准，比如代码中check函数中的参量int n，变量名改为number的话或许更有利于代码的可读性。

---
## 三、程序框架方面
该程序运用C++语言进行编写，框架较为清晰，先声明了需要使用的各个函数，再在之后完成了各函数的编写。

---
## 四、错误检测方面
该程序未设计错误检测，可能在输入有误时会引起不必要的麻烦。建议对输入进行判断，如果输入的不是0~9的数字，自动报错，并跳出程序。

---
## 五、改进反面
1. 在Input函数中，定义了一个二维字符数组进行输入，之后又将该二维字符数组转化成了二维整形数组。我认为完全没必要定义二维的字符数组temp，这样会导致程序冗余，直接用整形数组输入即可。
2. 整个代码的架构较为简单，功能较为单一，可以考虑之后不断优化，增加新的功能。

---
## 六、评价人
     姓名：卢沁书
     学号：U201611873