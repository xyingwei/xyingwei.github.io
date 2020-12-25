---
title: 函数Function
date: 2020-12-23
categories: TypeScript
cover: https://images.pexels.com/photos/3363359/pexels-photo-3363359.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260
---


## 一般函数
### 语法
  `function 函数名(): 返回值类型{}`
  ==必须定义返回值 没有返回值 定义为void==
### 示例
  ==形参和实参的类型和数量必须一致==
```
function jumpSan(param1, parm2) {
  console.log("\u5144\u5F1F\u4EEC,\u8DF3" + params + ",\u897F\u5317\u65B9" + parm2 + "\u7C73");
}
jumpSan('P城', 100);
```
## 可选参数的函数
### 语法
+ function 函数名(形参1:数据类型=默认值1,形参2:数据类型=默认值2):返回值类型{}
+ 传参:
  - 函数名(参数1) 
  - 函数名(参数1,参数2) 
  - 函数名(undefined,参数2)
### 示例
```
function buyGuns(params, param2, cont) {
  if (cont === void 0) { cont = 0; }
  console.log("\u4E70" + cont + "\u628A" + params + "," + param2);
}
buyGuns('ak47', 'm416', 10);
```
## 参数数量不确定的函数
### 语法
  function 函数名(形参1:类型,形参2:类型,...形参3:类型[]):void {}
  ==特点: 只能定义有一个 只能定义为数组 只能定义在形参最后==
### 示例
```
function add(x, y) {
    var resnumber = [];
    for (var _i = 2; _i < arguments.length; _i++) {
        resnumber[_i - 2] = arguments[_i];
    }
    // 创建一个求和变量
    var sum = x + y;
    // 使用for of语法 循环剩余参数
    for (var _a = 0, resnumber_1 = resnumber; _a < resnumber_1.length; _a++) {
        var item = resnumber_1[_a];
        sum += item;
    }
    console.log('和===', sum);
}
add(1, 2);
add(1, 2, 3, 4, 5, 6, 7);
```