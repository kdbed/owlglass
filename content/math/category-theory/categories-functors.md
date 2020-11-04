+++
title = "Categories, Functors, and Natural Transformations"
author = ["svejk"]
lastmod = 2020-11-03T23:19:27-05:00
draft = false
weight = 1
+++

## Category Theory Basics {#category-theory-basics}


### Category Theory and Mathematics {#category-theory-and-mathematics}

Category theory captures a number of essential features of mathematics. Mathematical theories often have a number of common ingredients: there are _objects_ -- numbers, sets, etc. -- and _arrows_ that provide relations among the objects.

-   a number is related to its divisors
-   functions relate sets

Furthermore, these relations can be composed.  In category theory, one has _objects_ and _arrows_, and results about these categories only make use of a single operation: composition of arrows. In this way, category theory ignores domain specific information, obtaining rich results that apply to every category.


### Basic Definitions {#basic-definitions}

Begin with the defintion of a category:

**Definition**  : A **category** \\(\mathcal{C} = (O,A,\circ)\\) consists of:

1.  a collection \\(O\\) of _objects_, written \\(a,b,... \in O\\)
2.  a collection \\(A\\) of _arrows_, written \\(f,g,... \in A\\) between these objects, e.g., $ f: a &rarr; b$
3.  a notion of _composition_ \\(f \circ g\\) of arrows
4.  an identity arrow \\(\text{id}\_a\\) for each object \\(a \in O\\)

The composition operation and identity arrow should satisfy the following laws:

-   _Composition_: If \\(f : a \rightarrow b\\) and \\(g : b \rightarrow c\\) then \\(g \circ f : a \rightarrow c\\).

{{< figure src="/images/cat1.png" >}}
