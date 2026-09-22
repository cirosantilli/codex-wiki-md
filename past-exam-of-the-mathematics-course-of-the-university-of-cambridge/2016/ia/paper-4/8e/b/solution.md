<h1 id="8e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the finite [binomial theorem](../../../../../../binomial-theorem.md) and set $z=1$. For $n\geq1$ this gives

$$
\boxed{\sum_{m=0}^n m\binom nm=n2^{n-1}}.
$$

For $n=0$ the sum is $0$ directly.

For the [alternating binomial moments](../../../../../../alternating-binomial-moment.md), it is useful to differentiate in a form that introduces [falling factorials](../../../../../../falling-factorial.md). Write $(m)_j=m(m-1)\cdots(m-j+1)$, with $(m)_0=1$. Differentiating the [binomial theorem](../../../../../../binomial-theorem.md) $j$ times and multiplying by $z^j$ yields, for $0\leq j\leq n$,

$$
\sum_{m=0}^n(m)_j\binom nm z^m=(n)_jz^j(1+z)^{n-j}.
$$

At $z=-1$, the right side vanishes when $j<n$, and equals $(-1)^nn!$ when $j=n$.

The [polynomials](../../../../../../polynomial-split.md) $(X)_0,\ldots,(X)_r$ have degrees $0,\ldots,r$ and leading coefficient $1$, so successive cancellation of leading terms expresses $X^r$ as a linear combination of them. If $r<n$, every falling-factorial term has index $j<n$ and hence its alternating sum vanishes. If $r=n$, the coefficient of $(X)_n$ is $1$, and all lower-index terms still vanish. Therefore **the alternating moments are**

$$
\boxed{S_r(n)=0\quad(0\leq r<n),\qquad S_n(n)=(-1)^nn!}.
$$

For $n=0$, the latter identity uses the constant polynomial $X^0=1$, so its value at $X=0$ is $1$; thus $S_0(0)=1$ as well. This makes the edge-case convention explicit rather than treating $0^0$ as an unrelated numerical expression.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
