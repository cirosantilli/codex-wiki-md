<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $a^{ij}=g^{ij}$, $r^2=|x|^2$, and $E=x\cdot\nabla$. The [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) from part (a) gives

$$
a^{ij}x_i=x_j,\qquad a^{ij}x_ix_j=r^2,\qquad\sum_{i,j}\partial_j(a^{ij}x_i)=n.
$$

For the Gaussian $q_t(x)=(4\pi t)^{-n/2}e^{-r^2/(4t)}$, we have $\partial_iq_t=-x_iq_t/(2t)$. Applying precisely the divergence-form operator in the paper yields

$$
Lq_t=-\partial_j(a^{ij}\partial_iq_t)
=\frac1{2t}\partial_j(x_jq_t)
=\left(\frac n{2t}-\frac{r^2}{4t^2}\right)q_t.
$$

Since $\partial_tq_t=(-n/(2t)+r^2/(4t^2))q_t$, the Gaussian itself already satisfies $(\partial_t+L)q_t=0$.

For completeness, the product rule gives for an arbitrary smooth $G$,

$$
(\partial_t+L)(q_tG)=q_t\left(\partial_tG+LG+\frac1t EG\right).
$$

Indeed the cross term in $L(q_tG)$ is $-2a^{ij}(\partial_iq_t)(\partial_jG)=q_t EG/t$. Substituting the [formal power series](../../../../../../formal-power-series.md) $G=\sum_{k\geq0}t^kB_k$, with $B_0=1$, gives the radial transport equations

$$
(E+k)B_k=-LB_{k-1},\qquad k\geq1.
$$

Along a radial segment their unique smooth solution is

$$
B_k(x)=-\int_0^1s^{k-1}(LB_{k-1})(sx)\,ds.
$$

The integral is smooth including at the centre, since each derivative adds a nonnegative power of $s$ to the integrable factor $s^{k-1}$. Uniqueness follows because a homogeneous solution $h$ has $d(s^kh(sx))/ds=0$; smoothness makes its limit at $s=0$ zero, so $h(x)=0$. This also excludes singular ray-dependent homogeneous solutions.

Here $L1=0$, so the recursion successively gives $\boxed{B_k=0\ (k\geq1),\quad G(x,t)=1}$. Thus both existence and uniqueness hold, with no convergence issue because the formal solution is the exact Gaussian. This is the [normal-coordinate divergence-form heat parametrix](../../../../../../normal-coordinate-divergence-form-heat-parametrix.md). The [positive Laplace-Beltrami operator](../../../../../../positive-laplace-beltrami-operator.md) $-\rho^{-1}\partial_j(\rho g^{ij}\partial_i)$, where $\rho=\sqrt{\det g}$, has an additional first-order term and a different leading amplitude; it is essential to use the operator actually specified here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
