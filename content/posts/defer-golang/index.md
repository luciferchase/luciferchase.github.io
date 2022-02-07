---
title: "What the heck is defer?"
date: 2022-01-31
draft: false

categories: ["articles"]
tags: ["Coding", "Golang"]

images: ["gopher.webp"]
featuredImage: gopher.webp
toc: false
---

Do you struggle to get the hang of `defer` too?\
Worry not :smile:, I will try to explain it as simply as I can in this post.

<!--more-->

{{< admonition type=info title="What is defer?" open=true >}}
A defer statement defers the execution of a function until the surrounding function returns.

The deferred call's arguments are evaluated immediately, but the function call is not executed until the surrounding function returns.
{{< /admonition >}}

This program explains the execution of `defer` in a bit easier way:

```go
func trace(s string) string {
    fmt.Println("entering:", s)
    return s
}

func un(s string) {
    fmt.Println("leaving:", s)
}

func a() {
    defer un(trace("a"))    // similarly trace("a") also gets
                            // executed immediately
    fmt.Println("in a")
}

func b() {
    defer un(trace("b"))    // trace("b") gets executed
                            // immediately but un("b") gets
                            // execute at the very last
    fmt.Println("in b")
    a()
}

func main() {
    b()
}
```

**Output:**

```go
entering: b     // output of trace("b")
in b            // note that un("b") is not executed instead
                // program moves ahead
entering: a     // output of trace("a")
in a
leaving: a      // finally defered un("a") is called as a()
                // returns
leaving: b      // at last un("b") is called
```

{{< admonition type=tip open=true >}}
Deferred function calls are pushed onto a stack.
When a function returns, its deferred calls are executed in last-in-first-out order.
{{< /admonition >}}

Here is a small program which visualises this:

```go
package main

import "fmt"

func main() {
    fmt.Println("counting \n")
    defer fmt.Println("\ndone")     // This will get executed at
                                    // the very last

    for i := 0; i < 10; i++ {
        defer fmt.Println(i)
    }
}
```

**Output:**

```go
counting

9
8
7
6
5
4
3
2
1

done
```

However remember deferred function's arguments are evaluated immediately, hence it can give a different result

```go
i := 0
defer fmt.Println(i)
i++

// It will print 0 even though i has become 1
```


A particularly good use of `defer` is to close a file.

```go
package main
import (
    "os"
)

func main() {
    f, _ := os.Create("test.txt")
    defer f.Close()
    /*
        Stuff
    */
}
```

{{< admonition type=abstract open=true >}}
Deferring a call to a function such as Close has two advantages. First, it guarantees that you will never forget to close the file, a mistake that's easy to make if you later edit the function to add a new return path.
Second, it means that the close sits near the open, which is much clearer than placing it at the end of the function.
[Source](https://go.dev/doc/effective_go#defer)
{{< /admonition >}}

{{< admonition type=tip open=true >}}
Read an in-depth article on `defer` to understand it better: [Defer, Panic, and Recover](https://go.dev/blog/defer-panic-and-recover)
{{< /admonition >}}
