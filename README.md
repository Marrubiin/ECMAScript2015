ES6学习笔记

1.变量let和const，使用let替代var，理解作用域。使用const申明常量。

2.do表达式，获取块级作用域的返回值

3.解构赋值：数组、对象、字符串、数值和布尔值、函数参数

用途：(1)交换变量的值 (2)函数返回多个值 (3)定义函数的参数 (4)提取JSON数据 (5)设置函数默认值 (6)遍历Map结构 (7)加载模块时指定方法
  
4.Unicode字符扩展，识别超出\u0000~\uFFFF之间的字符

(1)codePointAt()，返回指定位置的字符编码，codePointAt(0)返回特殊字符的完整编码，从1开始和charCodeAt()返回相同。es5的方法为charCodeAt()。

(2)String.fromCodePoint()，从码点返回对应字符，可识别32位的UTF-16字符(Unicode编号大于0xFFFF)，es5方法Strign.fromCharCode的扩展。

(3)字符串遍历方法for...of

(4)at()，返回字符串指定位置的字符，es5方法为charAt()。

(5)normalize()，统一字符的不同表示方法，Unicode正规化。

5.字符串查找方法：includes()、startWith()、endsWith()。

includes()：判断是否找到字符串，startWith()：判断字符串是否在原字符串头部，endsWith()：判断字符串是否在原字符串尾部。

三个方法都可使用第二个参数，表示开始搜索的位置。

6.repeated()，第一个参数为需要重复的字符串，第二个字符串为重复的次数。大-1的小数会自动取整，小于1的书或者Infinity会报错。NaN等于0。字符串会自动转换为数字。

7.padStart()，padEnd()：用指定字符串补齐到指定长度，第一个参数为长度，第二个为补齐字符串。省略第二个参数，会使用空格补齐。可指定字符串格式。

8.模板字符串，使用反引号表示（`），变量使用$()格式。取消换行或者空格格式，可以使用trim()方法

9.RegExp构造函数
