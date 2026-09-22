<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose $A_0$ lies on the relative boundary of $K$ in its span $L$. There is a nonzero $x\in L$ with $x^\top y\geq0$ for every $y\in K$ and $x^\top A_0=0$. Here is a direct construction of the supporting vector. Choose points $z_n\in L\setminus K$ converging to $A_0$, let $p_n$ be their nearest points in $K$, and set $x_n=(p_n-z_n)/\|p_n-z_n\|$. The minimization inequality for a nearest point gives $x_n^\top y\geq0$ on $K$ and $x_n^\top p_n=0$. A subsequence of the unit vectors converges to a unit vector $x\in L$. Since $0\leq x_n^\top A_0\leq\|A_0-z_n\|$, it has the asserted support properties.

The test-weight characterization of $K$ now gives $x^\top A_1\geq0$ almost surely. This random payoff cannot vanish almost surely: otherwise $x$ would annihilate every element of $D$, hence all of $L$, contradicting $x\in L$ and $\|x\|=1$. Therefore

$$
\boxed{x^\top A_0=0,\qquad x^\top A_1\geq0\text{ a.s.},\qquad P(x^\top A_1>0)>0.}
$$

This supplies the positive-terminal-payoff alternative. If $K$ has zero-dimensional span, its relative boundary is empty, so that case requires no supporting vector.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 41](../../../../paper-41-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
