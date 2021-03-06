+++
title = "Hello"
author = ["svejk"]
lastmod = 2021-03-05T22:42:34-05:00
draft = false
weight = 1
+++

## The Basics {#the-basics}


### Hello {#hello}

Begin with a simple hello world program <sup id="9959731cd3b000956d8cb62e5e556626"><a href="#kurt2018get" title="Kurt, Get Programming with Haskell, Manning Publications (2018).">kurt2018get</a></sup>:

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


### Messy Main {#messy-main}

To gain some intuition for the structure of Haskell programs, we introduce messyMain, which defies the good practice of writing modular code:

{{< highlight haskell "linenos=table, linenostart=1" >}}
--messyMain.hs : an example to fix
main :: IO()
main = do
    print "Who is the email for?"
    recipient <- getLine
    print "What is the Title?"
    title <- getLine
    print "Who is the Author?"
    author <- getLine
    print ("Dear " ++ recipient ++ ", \n" ++
          "Thanks for buying " ++ title ++ "\nthanks, \n" ++
          author )
{{< /highlight >}}
