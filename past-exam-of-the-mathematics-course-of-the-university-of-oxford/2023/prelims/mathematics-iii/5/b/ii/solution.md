<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an independent nonnegative integer-valued count $N$ and identically distributed independent summands, the [random sum probability generating function](../../../../../../../probability-generating-function-of-an-independent-random-sum.md) is $G_Z(s)=G_N(G_{X_1}(s))$. Conditioning on $N=n$ proves this, since the conditional [probability generating function](../../../../../../../probability-generating-function.md) is $G_{X_1}(s)^n$.

Here $G_{X_1}(s)=1-r+rs$, so

$$
\boxed{G_Z(s)=\frac p{1-(1-p)(1-r+rs)}=\frac p{p+(1-p)r-(1-p)rs}.}
$$

This identity holds throughout $|s|\leq1$, and its power-series extension has radius $[p+(1-p)r]/[(1-p)r]$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
