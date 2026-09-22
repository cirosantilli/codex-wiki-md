<h1 id="6c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The relevant one of the [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) is

$$
\rho(w)=w^3+(a-1)w-a=(w-1)(w^2+w+a).
$$

The coefficients on the right are chosen to give third order, so [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) is already available. By the [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md), convergence with convergent starting values is equivalent to [zero-stability](../../../../../../zero-stability.md): every root of $\rho$ must satisfy $|w|\leq1$, and every root on the unit circle must be simple.

If $a<0$, the quadratic is negative at $w=-1$ and tends to $+\infty$ as $w\to-\infty$, so it has a root less than $-1$. If $a>1$, its root product is $a$, so at least one root has modulus greater than one. For $0\leq a\leq1/4$, its real roots $(-1\pm\sqrt{1-4a})/2$ lie in $[-1,0]$. For $1/4<a\leq1$, its conjugate roots have modulus $\sqrt a\leq1$.

At $a=0$, the three roots are $1,0,-1$, with the unit-modulus roots simple. At $a=1$, they are $1,e^{2\pi i/3},e^{-2\pi i/3}$, again simple. The repeated quadratic root at $a=1/4$ is $-1/2$, strictly inside the unit circle, which the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) permits. Therefore

$$
\boxed{\text{the method is convergent exactly for }0\leq a\leq1.}
$$

This is the [root stability of a cubic multistep polynomial](../../../../../../root-stability-of-a-cubic-multistep-polynomial.md); oscillatory parasitic roots at the endpoints do not invalidate convergence when their starting amplitudes tend to zero.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6C](../../6c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
