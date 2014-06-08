---
layout: post
title: Bool Values in Swift
---

{{ page.title }}
================

In order to use your own custom types in expressions where a boolean value is required,
such as test part of `if` expressions, you need to implement `LogicValue` protocol.

So a useless random boolean type can be defined and used like this:

```
import Foundation

struct RandomBool: LogicValue {
  func getLogicValue() -> Bool {
    return Int(arc4random() % 2) == 0
  }
}

let b = RandomBool()
if b {
  println("b is true")
} else {
  println("b is false")
}
```
