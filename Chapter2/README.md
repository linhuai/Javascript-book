# 第二章 数组

判断一个变量是否为数组？
可靠地检测数组方法

### 1.利用Object的toString方法

```
var list = [1, 2, 3];
Object.prototype.toString.call(list); //[object Array]
```
### 2.利用ES5的Array.isArray()方法

```
var list = [1, 2, 3];
Array.isArray(list); //true
```
### 数组的原生方法有哪些？

**会改变自身的方法：**

copyWithin、fill、pop、push、reverse、shift、sort、splice、unshift

**不会改变自身的方法：**

concat、includes、join、slice、toSource、toString、indexOf、lastIndexOf

**遍历方法：**

forEach、entries、every、some、filter、find、findIndex

keys、map、reduce、reduceRight、values

**如何将类数组的变量转化为数组？**

如果是ES6，可以用Array.from()方法。

通常用Array.prototype.slice.call()的方法，将类似数组转换为数组。