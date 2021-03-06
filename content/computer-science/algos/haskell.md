+++
title = "Algorithms in Haskell"
author = ["svejk"]
lastmod = 2021-03-05T20:38:10-05:00
draft = false
weight = 1
+++

## Introduction {#introduction}

This is an introduction to the principles of algorithm design from a purely functional approach <sup id="a1f6e81b5f159280132e5c1de0f154aa"><a href="#bird_gibbons_2020" title="Bird \&amp; Gibbons, Algorithm Design with Haskell, Cambridge University Press (2020).">bird_gibbons_2020</a></sup>.  Using functions to express algorithms represents a dramatic shift from the imperative approach, as an algorithm expressed as a function is composed of other, more basic functions that can be studied separately and reused in other algorithms.  The properties of these functions and their relationship to others can be captured with simple equational properties.

To reason formally about imperative programs, one must formulate their specifications using the predicate calculus, using loop invariants to prove that they're correct.  However, one cannot easily reason about the properties of an imperative program directly in terms of the language of its code. Thus, there is usually a wide gap between books on formal program design and algorithm design.

A functional approach bridges this gap.

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
