# 便利的对象
本章，我们将介绍数组和散列(我们称为容器［container］)这两种新的数据结构。另外，我们还会介绍处理字符串时常用的工作——正则表达式。
##数组
数组（array）是一个按顺序保存多个对象的对象，它是基本的容器之一。
###数组的创建
需要把各数组的元素用逗号隔开，然后再用[]把他们括起来。
eg：names ＝ ［"小林","林","高野","森冈"］
###数组对象
###从数组从抽取对象
根据数组名索引进行抽取，索引值从0开始。
###将对象保存在数组中
数组名［索引］ ＝ 希望保存的对象
###数组的元素
任何对象都可以作为数组元素保存到数组中
###数组的大小
我们可以用size来查看数组的大小
数组名.size
###数组的循环
each方法（也称带块带方法）的语法如下：
  数组.each to ｜变量｜
     希望循环的处理
  end
do~~end之间懂部分称为块（block）；像“do~end”这样跨行的代码，输入end之前的代码是不会执行的。
##散列（hash）
散列也是一个程序里常用的容器。散列是键值对（key—value pair）的一种数据结构。在ruby中，一般是以字符串或者符号（symbol）作为键，来保存对应的对象。
###什么是符号
在ruby中，符号与字符串对象很相似，符号也是对象，一般作为名称标签来使用。符号和字符串可以相互任意转换。对符号使用to_sd方法，则可以得到相应的字符串。反之亦然。
###散列的创建
用{}把创建的内容括起来。散列用=>来定义获取对象时所需的键（key），以及键对应的对象（value）。
eg：address = {:name => "高桥",:pinyin => "gaoqiao"} 当符号当作键是，也可以写成 address = {name: "高桥",:pinyin: "gaoqiao"}
###散列的使用
###散列的循环
  散列.each to ｜键变量，值变量｜
     希望循环的处理
  end
##正则表达式
使用其可以实现一下功能：
将字符串与模式相匹配；使用模式分割字符串
###模式与匹配
匹配：判断字符串是否适用于某模式的过程称为匹配
eg：/cde/ =~ "abcdefgh"
创建正则表达式的语法： /模式/；/模式/i指不区分大小写。
匹配正则表达式与字符串的方法：/模式/ =~ "希望匹配的字符串"
字符串的首个字符位置为0，匹配失败则返回nil。
##nil
nil是一个特殊的值，表示对象不存在。

###


