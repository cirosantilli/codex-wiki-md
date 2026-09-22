<h1 id="9f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking the [matrix trace](../../../../../../matrix-trace.md) of the adjugate expansion and using part (b) gives

$$
\sum_{i=0}^{n-1}\operatorname{Tr}(B_i)t^{n-1-i}
=\sum_{i=0}^{n-1}(n-i)c_it^{n-1-i}.
$$

Hence $\operatorname{Tr}(B_i)=(n-i)c_i$. Taking traces in $B_i=AB_{i-1}+c_iI$ gives, for $1\leq i<n$,

$$
c_i=-\frac1i\operatorname{Tr}(AB_{i-1}).
$$

For $i=n$, the same formula follows by taking the trace of $-AB_{n-1}=c_nI$. Iterating the recursion from part (a) also gives

$$
B_{i-1}=A^{i-1}+c_1A^{i-2}+\cdots+c_{i-1}I.
$$

Consequently the [Faddeev–LeVerrier algorithm](../../../../../../faddeev-leverrier-algorithm.md) is

$$
\boxed{c_i=-\frac1i\left[\operatorname{Tr}(A^i)
+c_1\operatorname{Tr}(A^{i-1})+\cdots+c_{i-1}\operatorname{Tr}(A)\right],
\quad1\leq i\leq n}.
$$

Starting with $c_0=1$, this recursively expresses every $c_i$ using only $\operatorname{Tr}(A),\ldots,\operatorname{Tr}(A^i)$; these are the [Newton identities](../../../../../../newton-s-identities.md) for the [characteristic polynomial](../../../../../../characteristic-polynomial.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
