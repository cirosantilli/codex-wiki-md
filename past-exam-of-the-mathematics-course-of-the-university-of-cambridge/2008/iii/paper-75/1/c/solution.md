<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $d$ be the dimension of a proposed real [Chebyshev system](../../../../../../chebyshev-system.md) on the circle, and regard its [functions](../../../../../../function-split.md) as continuous $2\pi$-periodic [functions](../../../../../../function-split.md) on the real line. Choose lifted points $\theta_0<\theta_1<\cdots<\theta_{d-1}<\theta_0+2\pi$ and set $\theta_d=\theta_0+2\pi$. Move the points by

$$
\theta_i(s)=(1-s)\theta_i+s\theta_{i+1},\qquad 0\le s\le1,\quad 0\le i<d.
$$

For every $s$ the points remain distinct on the circle. Indeed, each consecutive gap is a convex combination of positive gaps; the closing gap is also a convex combination of the original closing gap and $\theta_1-\theta_0$. The evaluation [determinant](../../../../../../determinant.md)

$$
D(s)=\det(u_j(\theta_i(s)))_{i,j=0}^{d-1}
$$

is therefore nonzero for every $s$ by the [determinant criterion for a Chebyshev system](../../../../../../determinant-criterion-for-a-chebyshev-system.md). It is continuous, so the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) forbids a sign change. At $s=1$, however, periodicity makes its rows the cyclic permutation of the initial rows, giving $D(1)=(-1)^{d-1}D(0)$. For even $d$ this reverses the sign, a contradiction. Hence **every such periodic Chebyshev system has odd dimension; none has even dimension**. This [determinant](../../../../../../determinant.md) argument avoids assuming differentiability or simple zeros of the [functions](../../../../../../function-split.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
