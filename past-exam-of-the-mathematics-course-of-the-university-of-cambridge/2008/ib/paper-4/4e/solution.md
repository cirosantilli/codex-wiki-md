<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

Set $h=f-g$, an [entire function](../../../../../entire-function.md). By the [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md), a subsequence of the distinct zeros $z_i$ converges to a point $a$ in the closed unit disc. An [analytic function](../../../../../space-of-holomorphic-functions.md) has a convergent [Taylor series](../../../../../taylor-series.md) in a neighbourhood of each point. If the first nonzero coefficient of $h$ at $a$ had index $m$, then

$$
h(z)=(z-a)^m k(z),\qquad k(a)\neq0,
$$

with $k$ analytic and nonzero in a sufficiently small disc. The zero $a$ would then be isolated, contradicting the accumulating distinct zeros. All Taylor coefficients at $a$ vanish, so $h$ vanishes on a disc.

To justify continuation across the whole plane, let $Z$ be the set of points at which $h$ vanishes on a neighbourhood. This set is nonempty and open. It is also closed: if points of $Z$ tend to $b$, continuity of each derivative gives $h^{(m)}(b)=0$ for every $m$, and the [Taylor series](../../../../../taylor-series.md) at $b$ gives a zero neighbourhood. Since $\mathbb C$ is a [connected space](../../../../../connected-space.md), $Z=\mathbb C$. This proves the [identity theorem](../../../../../identity-theorem.md) here and gives $\boxed{f\equiv g}$.

Without boundedness, the distinct zeros need not have an accumulation point in the plane. For example,

$$
\boxed{f(z)=\sin(\pi z),\qquad g(z)=0,\qquad z_i=i\ (i=1,2,\ldots)}
$$

are distinct [entire functions](../../../../../entire-function.md) agreeing at all the indicated positive integers.

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
