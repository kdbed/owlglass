+++
title = "Hello"
author = ["svejk"]
lastmod = 2021-02-21T22:32:49-05:00
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

{{< highlight shell "linenos=table, linenostart=1" >}}
ghc hello.hs
{{< /highlight >}}

```text
[1 of 1] Compiling Main             ( hello.hs, hello.o )
Linking hello ...
```

Thus GHC has created three files: **hello**, the binary executable, along with hello.hi and hello.o.  The binary can be executed from the command line:

{{< highlight shell "linenos=table, linenostart=1" >}}
./hello
{{< /highlight >}}

```text
"Hello World!"
```
