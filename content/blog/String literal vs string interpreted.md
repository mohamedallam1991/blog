---
title: "Strings literal vs string interpreted"
date: 2023-03-24
description: "The subtile difference between string literal versus string interpreted in Golang's terminology"
tags: ["golang","string", "strings"]
showTableOfContents: true
draft: false
---


A string literal is a string, without any formatting or anything to it, its literal as it says, so we use the back ticks for string literals, by that nothing we can type within the string to that would be printing differently than what we put between the back ticks

```go
literalString := `some words\n or #vs`
```

## string interpreted
Go, when we use double quptes, we are telling go its an interpreted string, uses some of the formatting that look familiar if you are coming from C language , for example a string can have a new line, by simply using slash n, or other verbs like that, the documentation on Go explains different verbs and keywords we can use in interpreted strings

```go
interpretedString := "interpreted string"
```
