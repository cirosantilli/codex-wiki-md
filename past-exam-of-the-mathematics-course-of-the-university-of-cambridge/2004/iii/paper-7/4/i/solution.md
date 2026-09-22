<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The defining [convolution](../../../../../../convolution.md) integral is absolutely convergent for every $x$ when $e\in L^1+L^2$. Indeed, writing $e=a+b$ with $a\in L^1$ and $b\in L^2$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\int|K(x-y)e(y)|\,dy\leq\|K\|_\infty\|a\|_1+\|K\|_2\|b\|_2<\infty.
$$

Disjoint supports imply $\sum_n|e_n(y)|=|e(y)|$ almost everywhere. The [Tonelli theorem](../../../../../../tonelli-theorem.md) therefore yields

$$
\sum_n\int|K(x-y)e_n(y)|\,dy=\int|K(x-y)e(y)|\,dy<\infty.
$$

We may exchange the sum and integral; the resulting numerical series is absolutely convergent. Its [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\boxed{|T(e)(x)|\leq\sum_n|T(e_n)(x)|.}
$$

Here $e$ belongs to the stated operator domain, as is implicit when writing $T(e)$. Disjoint supports also ensure that each summand belongs to that domain.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
