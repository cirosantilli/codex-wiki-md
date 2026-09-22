<h1 id="18d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With $\rho_0=a$, $\rho_1=\theta$, $\rho_2=1$, the constant order condition gives $a=-1-\theta$. The next three [order conditions for a linear multistep method](../../../../../../order-conditions-for-a-linear-multistep-method.md) give

$$
\theta+2=\sigma_0+\sigma_1+\sigma_2,\qquad \theta+4=2\sigma_1+4\sigma_2,\qquad \theta+8=3\sigma_1+12\sigma_2.
$$

Solving this linear system yields **the unique coefficients of order at least three**:

$$
\boxed{a=-1-\theta,\qquad \sigma_0=\frac{5\theta+4}{12},\quad \sigma_1=\frac{2(\theta+2)}3,\quad \sigma_2=\frac{4-\theta}{12}.}
$$

The characteristic polynomial controlling [zero-stability](../../../../../../zero-stability.md) factors as

$$
\rho(\zeta)=\zeta^2+\theta\zeta-1-\theta=(\zeta-1)(\zeta+1+\theta).
$$

The other root is $-1-\theta$. Requiring its modulus to be at most one gives $-2\leq\theta\leq0$, but $\theta=-2$ produces a repeated root at one and violates the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md). At $\theta=0$, the roots $1,-1$ are both simple, so that endpoint is allowed. By the [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md), **the method converges precisely for**

$$
\boxed{-2<\theta\leq0.}
$$

The fourth defect coefficient is $C_4=\theta$, so the method has order exactly three for nonzero $\theta$. At $\theta=0$ it is the two-step Simpson method, of order four; thus the extra-order endpoint has correctly remained in the answer.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [18D](../../18d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
