<h1 id="4/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For the linear evolution from part (iii), maximize the energy ratio at each time. The [optimal energy amplification of a linear system](../../../../../../../optimal-energy-amplification-of-a-linear-system.md) is

$$
G_{\rm opt}(t)=\max_{x_0\ne0}\frac{\|M(t)x_0\|^2}{\|x_0\|^2}
=\sigma_{\max}(M(t))^2
=\frac{S+\sqrt{S^2-4a^2d^2}}2,\qquad S=a^2+b^2+d^2.
$$

Thus the optimizing initial state is a [right singular vector](../../../../../../../right-singular-vector.md), not generally an [eigenvector](../../../../../../../eigenvector.md) of $L$.

There is a convenient exact way to find the maximizing time. Let $x_0$ be a unit optimizing initial vector and $y=M(t)x_0$. The [singular value decomposition](../../../../../../../singular-value-decomposition.md) gives $M^Ty=G_{\rm opt}x_0$. For $t>0$, the top singular value is simple. At an interior time maximum,

$$
0=\frac12G_{\rm opt}'(t)=y^TLy.
$$

Since $LM=ML$, this also equals $G_{\rm opt}x_0^TLx_0$. Thus both initial and final orientations are neutral energy-growth directions. The positive entries of $M^TM$ let the top [right singular vector](../../../../../../../right-singular-vector.md) be chosen with positive components. Its orientation decreases through the growth sector, so it must start at $\rho^+$ and end at $\rho^-$.

Put $q=a/d=e^{-3t/(4R)}$ and $K=4R/3$. The solution gives

$$
\rho(t)=\frac{\rho^+}{q+K\rho^+(1-q)}.
$$

Setting this equal to $\rho^-$ yields

$$
q_* =\frac{\rho^+(1-K\rho^-)}{\rho^-(1-K\rho^+)}
=\frac{5-3s}{5+3s},\qquad s=\sqrt{1-R^{-2}}.
$$

Therefore **the exact optimal time for $R>1$ is**

$$
\boxed{T^*=\frac{4R}{3}\log\frac{5+3\sqrt{1-R^{-2}}}{5-3\sqrt{1-R^{-2}}}.}
$$

Here and below $\log$ is the natural logarithm. This is the unique positive stationary time: $q$ decreases monotonically from one to zero, and the neutral-direction condition determines one $q_*\in(0,1)$. Also $G_{\rm opt}(0)=1$, $G_{\rm opt}(\infty)=0$, and $R>1$ admits initial energy growth, so this stationary point is the global maximum. For $R\leq1$, the [instantaneous energy-growth criterion for a linear system](../../../../../../../instantaneous-energy-growth-criterion-for-a-linear-system.md) gives no amplification, and the maximum is one at time zero.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
