+++
title = "Algorithms in Haskell"
author = ["svejk"]
lastmod = 2021-03-05T21:27:12-05:00
draft = false
weight = 1
+++

## Introduction {#introduction}

This is an introduction to the principles of algorithm design from a purely functional approach <sup id="a1f6e81b5f159280132e5c1de0f154aa"><a href="#bird_gibbons_2020" title="Bird \&amp; Gibbons, Algorithm Design with Haskell, Cambridge University Press (2020).">bird_gibbons_2020</a></sup>.  Using functions to express algorithms represents a dramatic shift from the imperative approach, as an algorithm expressed as a function is composed of other, more basic functions that can be studied separately and reused in other algorithms.  The properties of these functions and their relationship to others can be captured with simple equational properties.

To reason formally about imperative programs, one must formulate their specifications using the predicate calculus, using loop invariants to prove that they're correct.  However, one cannot easily reason about the properties of an imperative program directly in terms of the language of its code. Thus, there is usually a wide gap between books on formal program design and algorithm design.

A functional approach bridges this gap.
