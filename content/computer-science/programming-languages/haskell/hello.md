+++
title = "Hello"
author = ["svejk"]
lastmod = 2021-02-10T23:39:22-05:00
draft = false
weight = 1
+++

## The Basics {#the-basics}


### Hello {#hello}

Begin with a simple hello world program:

<a id="code-snippet--hello.hs"></a>
```haskell
--hello.hs : first haskell file
main = do
  print "Hello World!"
```

Compile the code by passing <span class="underline">hello.hs</span> to GHC as an argument:

```shell
ghc hello.hs
```

```text
[1 of 1] Compiling Main             ( hello.hs, hello.o )
Linking hello ...
```
