<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [dispersion relation](../../../../../../dispersion-relation.md) has two additional arguments with the same value. Indeed,

$$
\omega(\nu)=\omega(k)\quad\Longleftrightarrow\quad
(\nu-k)(\nu^2+k\nu+k^2-1)=0.
$$

Thus use the [cubic Stokes dispersion symmetry](../../../../../../cubic-stokes-dispersion-symmetry.md)

$$
\nu_{1,2}(k)=\frac{-k\pm\sqrt{4-3k^2}}2,
\qquad \nu_1+\nu_2=-k,\quad\nu_1\nu_2=k^2-1.
$$

Both roots are in the lower half-plane for $k\in D_+$. At $k=iv$, $v>0$, their imaginary parts are $-v/2$. A root cannot cross the real axis in $D_+$, since a real root would make $\operatorname{Re}\omega(k)=\operatorname{Re}\omega(\nu)=0$. Continuity therefore proves the claim throughout this connected domain. The branch points $\pm2/\sqrt3$ are outside $\overline{D_+}$; interchanging the two root labels does not change the formula below.

Evaluate the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) at each $\nu_j$, where its analyticity requirement holds:

$$
i\nu_jG_1+G_2=e^{\omega t}\widehat q(\nu_j,t)-\widehat q_0(\nu_j)-(1-\nu_j^2)G_0.
$$

The left side is linear in $\nu_j$. Interpolate it to the argument $k$ with weights

$$
A_1(k)=\frac{k-\nu_2}{\nu_1-\nu_2},\qquad
A_2(k)=\frac{\nu_1-k}{\nu_1-\nu_2}.
$$

They satisfy $A_1+A_2=1$ and $A_1\nu_1+A_2\nu_2=k$. Hence

$$
B(k,t)=e^{\omega t}\sum_{j=1}^2 A_j\widehat q(\nu_j,t)
-\sum_{j=1}^2A_j\widehat q_0(\nu_j)+(1-3k^2)G_0.
$$

For the last coefficient, use

$$
A_1\nu_1^2+A_2\nu_2^2=k(\nu_1+\nu_2)-\nu_1\nu_2=1-2k^2;
$$

adding $1-k^2$ and subtracting the interpolated $1-\nu_j^2$ gives $1-3k^2$.

The remaining solution-transform contribution is $\int_{\partial D_+}e^{ikx}\sum_jA_j\widehat q(\nu_j,t)\,dk$. Its [integrand](../../../../../../integrand.md) is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) in $D_+$: the transformed arguments remain in the lower half-plane. The weights are bounded at infinity, and $e^{ikx}$ supplies decay on the upper closing arc for $x>0$. The [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) therefore makes this [integral](../../../../../../integral.md) zero. Put

$$
F(k)=A_1(k)\widehat q_0(\nu_1(k))+A_2(k)\widehat q_0(\nu_2(k)).
$$

The [Dirichlet spectral representation for the linear dispersive Stokes equation](../../../../../../dirichlet-spectral-representation-for-the-linear-dispersive-stokes-equation.md) is now

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega(k)t}\widehat q_0(k)\,dk
+\frac1{2\pi}\int_{\partial D_+}e^{ikx-\omega(k)t}\bigl[(1-3k^2)G_0(k,t)-F(k)\bigr]dk.}
$$

All quantities in this expression are transforms of the prescribed initial and boundary values. Neither derivative trace remains.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
