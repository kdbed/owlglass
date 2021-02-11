+++
title = "Hello"
author = ["svejk"]
lastmod = 2021-02-11T09:09:02-05:00
draft = false
weight = 1
+++

## The Basics {#the-basics}


### Hello {#hello}

Begin with a simple hello world program:

{{< highlight haskell "linenos=table, linenostart=1" >}}
--hello.hs : first haskell file
main = do
  print "Hello World!"
{{< /highlight >}}

Compile the code by passing **hello.hs** to GHC as an argument:

```shell
ghc hello.hs
```

```text
[1 of 1] Compiling Main             ( hello.hs, hello.o )
Linking hello ...
```
