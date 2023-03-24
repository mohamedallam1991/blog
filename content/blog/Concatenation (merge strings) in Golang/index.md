---
title: "Strings concatenation in Golang (merge strings)"
date: 2023-03-24
description: "an iconic example of how simple Golang is, example of concatenation of strings"
tags: ["golang","string", "strings"]
showTableOfContents: true
draft: false
---
In [Golang](../../Golang.md), [string](../String.md) are
in Go, concatenating strings is fairly easy and straight forward, you simply use the add or addition symbol and you are all set. and here is an example

![](94269f909a88fb1ba79fa1789d6170d4c9333d0b.png)

``` go
func concatenate() {
    firstName := "Mohamed"
    lastName := "Allam"
    fullName := firstName + lastName
    fmt.Println(fullName)
}
```

Or you can [try it yourself](https://go.dev/play/p/g75JTwTH-xq)

Strings are arrays, so you can use indexing as well,

``` go
firstName := "Mohamed"
firstLetter := firstName[0] // returns M
lnFirstLetter := "Allam"[0] // return A
```
