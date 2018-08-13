# Big O Notation

Big O Notation is sometimes referred to as **order of growth** - how does the
performance of an algorithm scale with the size of the input.

It is less useful to talk about the running time of an algorithm because the
same algorithm can run in different times on different machines or language
implementations, so we instead talk about the algorithm's **growth rate**.

If we have functions `f, g` such that `f` eventually grows slower than `g` for
some input we say that `f = O(g)`. `f` is `Big O` of `g`.
