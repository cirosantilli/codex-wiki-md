<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $E(t)=\int_{B_t(x_0)}|\nabla u|^2$. For $n\geq2$, choose $c$ in the [annular Caccioppoli inequality](../../../../../../annular-caccioppoli-inequality.md) to be the [integral average](../../../../../../integral-average.md) of $u$ over $A_R$. The supplied [Poincare inequality on an annulus](../../../../../../poincare-inequality-on-an-annulus.md) gives

$$
E(R)\leq C_1R^{-2}\int_{A_R}|u-c|^2\leq C_2\int_{A_R}|\nabla u|^2=C_2\bigl(E(2R)-E(R)\bigr).
$$

Moving the $E(R)$ term to the left is the [hole-filling argument](../../../../../../hole-filling-argument.md):

$$
E(R)\leq\theta E(2R),\qquad\theta=\frac{C_2}{1+C_2}\in(0,1).
$$

Consequently $E(2^{-k}r_0)\leq\theta^kE(r_0)$. Put $\beta=-\log_2\theta>0$ and choose $\mu=\min\{\beta/2,1/2\}\in(0,1)$. For $2^{-k-1}r_0<r\leq2^{-k}r_0$, monotonicity gives

$$
E(r)\leq\theta^kE(r_0)\leq2^{-k\mu}E(r_0)\leq2^\mu(r/r_0)^\mu E(r_0).
$$

Dyadic endpoints can be assigned to either adjacent interval. Since $E(r_0)\leq\int_B|\nabla u|^2$, the requested [dyadic energy decay](../../../../../../dyadic-energy-decay.md) is

$$
\boxed{E(r)\leq K(r/r_0)^\mu\int_B|\nabla u|^2,\qquad K=2^\mu.}
$$

Both constants depend only on the dimension and [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) bounds, not on $u,x_0,r,r_0$.

There is a dimensional detail in the printed hint: an [annulus](../../../../../../annulus-mathematics.md) is disconnected in dimension one, so that [Poincaré inequality](../../../../../../poincare-inequality.md) with a single average is false there. The conclusion still holds. In one dimension the weak equation gives $a(x)u'(x)=J$ almost everywhere for a [constant flux for a one-dimensional divergence-form equation](../../../../../../constant-flux-for-a-one-dimensional-divergence-form-equation.md) $J$. Since $\lambda\leq a\leq\Lambda$,

$$
E(r)\leq\frac{2rJ^2}{\lambda^2},\qquad E(r_0)\geq\frac{2r_0J^2}{\Lambda^2},\qquad E(r)\leq(\Lambda/\lambda)^2(r/r_0)E(r_0).
$$

This implies the required estimate with, for example, $\mu=1/2$ and $K=(\Lambda/\lambda)^2$. If $J=0$, the estimate is immediate. Thus the proof also covers dimension one without using the inapplicable hint.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
