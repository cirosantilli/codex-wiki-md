<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $D>0$ be the diameter of the bounded set $S$, and choose $x_0\in S$. Then $S\subseteq B(x_0,D)$. It is enough to prove a [volumetric covering bound](../../../../../../volumetric-covering-bound.md) for the unit ball.

Choose a maximal $1/4$-separated set $N$ in $B(0,1)$. The balls of radius $1/8$ centred at points of $N$ are disjoint and lie in $B(0,9/8)$. Comparing [volumes](../../../../../../lebesgue-measure.md) gives

$$
|N|\left(\frac18\right)^n\leq\left(\frac98\right)^n,
\qquad |N|\leq9^n.
$$

Maximality means that the balls of radius $1/4$ centred at $N$ cover the unit ball.

After translating and scaling, at most $9^n$ balls of radius $D/4$ cover $S$. Assign each point of $S$ to one covering ball containing it. This gives at most $9^n$ disjoint pieces, each of diameter at most $D/2<D$. Thus the claim holds with the absolute constant $C=9$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
