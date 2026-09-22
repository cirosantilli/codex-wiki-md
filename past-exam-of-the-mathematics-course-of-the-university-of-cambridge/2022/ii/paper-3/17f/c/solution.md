<h1 id="17f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Enumerate the vertices as $v_1,v_2,\ldots$. Since every vertex has finite degree, choose increasing finite vertex sets $W_n$ whose union is $V$ and such that the closed neighbourhood of $v_i$ lies in $W_n$ whenever $i\leq n$. By part (b), each finite induced graph $G[W_n]$ has an unfriendly two-colouring.

There are only two colours. Pass successively to an infinite subsequence on which the colour of $v_1$ is constant, then one on which the colour of $v_2$ is constant, and so on. The [diagonal argument](../../../../../../diagonal-argument.md) gives a limiting colouring in which, for every fixed finite set of vertices, all its colours agree with those in infinitely many of the finite colourings.

Fix $v_i$. Its entire finite neighbourhood lies in every sufficiently large $W_n$, and along the diagonal subsequence the colours of $v_i$ and all its neighbours eventually stabilize. The unfriendly inequality for $v_i$ in $G[W_n]$ therefore passes unchanged to the limit. This holds for every vertex, proving the [unfriendly partition theorem for a countable locally finite graph](../../../../../../unfriendly-partition-theorem-for-a-countable-locally-finite-graph.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17F](../../17f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
