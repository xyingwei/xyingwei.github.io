---
title: 类Class
date: 2020-12-22
categories: TypeScript
---

## Class
+ 封装
+ 继承
+ 多态

## 回顾以前创建对象方法
    构造函数 + new

## Class创建对象

```
class Animal {
  name: string;
  constructor(theName: string) { this.name = theName; }
  move(distanceInMeters: number = 0) {
    console.log(`${this.name} moved ${distanceInMeters}m.`);
  }
}
```
## 类的继承
```
class Snake extends Animal {
  constructor(name: string) { super(name); }
  move(distanceInMeters = 5) {
    console.log("Slithering...");
    super.move(distanceInMeters);
  }
}
```
```
class Horse extends Animal {
  constructor(name: string) { super(name); }
  move(distanceInMeters = 45) {
    console.log("Galloping...");
    super.move(distanceInMeters);
  }
}
```
## 实例化 调用
```
let sam = new Snake("Sammy the Python");
let tom: Animal = new Horse("Tommy the Palomino");

sam.move();
tom.move(34);
```


## code practice
```
class City {
  cname:string;
  clevel:number;
  constructor(cname:string,clevel:number){
    this.cname = cname;
    this.clevel = clevel;
  }
  about(){
    console.log(`欢迎来到${this.cname},危险系数为${this.clevel}`);
  }
}

// 创建对象
let c1 = new City('p城',5);
console.log(c1.cname);
c1.about();
```



