+++
title = "Logic and Proof - Introduction"
author = ["svejk"]
lastmod = 2020-11-10T14:50:11-05:00
draft = false
weight = 1
+++

## Mathematical Proof {#mathematical-proof}

The birth of mathematics proper is often placed in ancient Greece around the sixth century BC, when deductive proof was first introduced. It was perhaps Thales of Miletus who deserves credit for recognizing the importance of not just what we know but how we know it; he found grounds for knowledge in the deductive method. Euclid later codified a deductive approach to geometry in his <span class="underline">Elements</span>, and the axiomatic style set a paradigm for rigorous argumentation.


### Lean Proof {#lean-proof}

```lean
constant and : Prop → Prop → Prop
constant or : Prop → Prop → Prop
constant not : Prop → Prop
constant implies : Prop → Prop → Prop

variables p q r : Prop
#check and p q                      -- Prop
#check or (and p q) r               -- Prop
#check implies (and p q) (and q p)  -- Prop
```

```python
print(2+2)
```
