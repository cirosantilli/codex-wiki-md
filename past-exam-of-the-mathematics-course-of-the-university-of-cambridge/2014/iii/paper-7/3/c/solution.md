<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $T$ and set $A_T=\sup_{0\leq s\leq T}\|f(s)\|_1$. The preceding [integral](../../../../../../integral.md) estimate gives the result for one iterate. If for some $n\geq0$ the bound $\|\tau^nf(s)\|_1\leq A_T2^ns^n/n!$ holds for $s\leq T$, then

$$
 \|\tau^{n+1}f(t)\|_1\leq2\int_0^t\|\tau^nf(s)\|_1\,ds
 \leq\frac{2^{n+1}A_T}{n!}\int_0^t s^n ds
 =\frac{2^{n+1}t^{n+1}}{(n+1)!}A_T.
$$

Taking $T=t$ yields exactly

$$
 \boxed{\|\tau^nf(t)\|_1\leq\frac{(2t)^n}{n!}
 \sup_{0\leq s\leq t}\|f(s)\|_1.}
$$

The case $n=0$ uses the identity operator. This [factorial bound for a Volterra iterate](../../../../../../factorial-bound-for-a-volterra-iterate.md) comes from time ordering, so no commutation between free transport and the collision projection is assumed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
