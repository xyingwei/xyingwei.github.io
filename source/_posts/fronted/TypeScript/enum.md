---
title: 枚举Enum
date: 2020-12-22
categories: TypeScript
cover: https://w.wallhaven.cc/full/r7/wallhaven-r786xw.jpg
---

## 枚举 enum
```
enum Gender {
  Boy = 1,
  Girl = 2,
  Unknown = 3,
}
console.log(Gender.Boy)
console.log(Gender.Girl)
console.log(Gender.Unknown)

let useSex: Gender = Gender.Boy

console.log(useSex) // 1
```