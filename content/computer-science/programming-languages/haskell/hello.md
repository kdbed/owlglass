+++
title = "Hello"
author = ["svejk"]
lastmod = 2021-02-10T23:01:18-05:00
draft = false
weight = 1
+++

:ID:       42897f99-ec4f-48ec-8d7d-7022ef58ccb3


## The Basics {#the-basics}


### Hello {#hello}

Begin with a simple hello world program:

```haskell
--hello.hs : first haskell file
main = do
  print "Hello World!"
```

Compile the code by passing <span class="underline">hello.hs</span> to GHC as an argument:

```bash
ghc hello.hs
```
