<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Only $\alpha>0$ needs consideration, by the preceding [zero-stability](../../../../../../zero-stability.md) analysis. On the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), all roots of the [amplification polynomial](../../../../../../amplification-polynomial-of-a-multistep-method.md)

$$
P_z(\zeta)=\rho(\zeta)-z\sigma(\zeta)
$$

must satisfy the unit-disk root condition if the method is [A-stable](../../../../../../a-stability.md). Evaluate it at $\zeta=-1$:

$$
P_z(-1)=8+2\alpha z.
$$

Take a real negative $z<-4/\alpha$. Then $P_z(-1)<0$, whereas the leading coefficient $2+\alpha-z$ is positive and $P_z(\zeta)\to+\infty$ as $\zeta\to-\infty$. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) gives a real root strictly below $-1$. Its numerical mode grows in modulus, contradicting [absolute stability](../../../../../../linear-stability-domain.md) at this negative test parameter. Consequently

$$
\boxed{\text{no parameter gives both convergence and A-stability}.}
$$

This proof detects an unstable root directly; the second-order value alone would not exclude [A-stability](../../../../../../a-stability.md). Equivalently the limiting derivative polynomial has an exterior root $-\alpha-\sqrt{1+\alpha^2}$, explaining the instability for large negative $z$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
