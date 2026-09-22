<h1 id="7e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Given any $z\in\mathbb C$ that is not a nonpositive integer, choose $N$ large enough that $\operatorname{Re}(z+N)>0$ and define

$$
\boxed{
I(z)=\frac{I(z+N)}
{z(z+1)\cdots(z+N-1)}}.
$$

The recurrence shows that definitions from different sufficiently large $N$ agree, so this gives the unique [analytic continuation](../../../../../../analytic-continuation.md) from the right half-plane. It is analytic except where a denominator factor vanishes, namely

$$
\boxed{z=0,-1,-2,\ldots}.
$$

These points are [simple poles](../../../../../../simple-pole.md). More precisely, at $z=-n$,

$$
\operatorname*{Res}_{z=-n}I(z)
=\frac{(-1)^n}{n!},
$$

because one may write

$$
I(z)=\frac{I(z+n+1)}{z(z+1)\cdots(z+n)}
$$

and use $I(1)=1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7E](../../7e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
