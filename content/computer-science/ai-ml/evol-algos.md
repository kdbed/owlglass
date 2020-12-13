+++
title = "Introduction"
author = ["svejk"]
lastmod = 2020-11-13T10:11:15-05:00
draft = false
weight = 5
+++

## Genetic Algorithms {#genetic-algorithms}

Genetic algorithms <sup id="2db21128661cac95ad635fa85cdb03e0"><a href="#sheppard2016genetic" title="Sheppard, Genetic Algorithms with Python, CreateSpace Independent Publishing Platform (2016).">sheppard2016genetic</a></sup> use random exploration of the problem space along with evolutionary processes, e.g., mutation and crossover, to improve guesses.  With no knowledge in the problem domain, they may aid in understanding the problem space and potential solutions. Here is an example for password guessing.  Start with a randomly-generated initial sequence of letters, then mutate one random letter at a time until the sequence is "Hello World!".

Pseudocode:

```text
_letters = [a..zA..Z !]
target = "Hello World!"
guess = get 12 random letters from _letters
while guess != target:
    index = get random value from [0..length of target]
    guess[index] = get 1 random value from _letters
```

# Bibliography
<a id="sheppard2016genetic"></a>Sheppard, C., *Genetic algorithms with python* (2016), : CreateSpace Independent Publishing Platform. [↩](#2db21128661cac95ad635fa85cdb03e0)
