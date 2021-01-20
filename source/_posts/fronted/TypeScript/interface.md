---
title: 接口interface
date: 2020-12-30
categories: TypeScript
cover: https://w.wallhaven.cc/full/r7/wallhaven-r786xw.jpg
---

## 接口interface
`接口的作用就是为这些类型命名和为你的代码或第三方代码定义契约。`

## 示例
```
interface LabelledValue {
  label: string;
}
function printLabel(labelledObj:LabelledValue) {
  console.log(labelledObj.label)
}
et myObj = {size: 10, label: "Size 10 Object"};
printLabel(myObj);
```