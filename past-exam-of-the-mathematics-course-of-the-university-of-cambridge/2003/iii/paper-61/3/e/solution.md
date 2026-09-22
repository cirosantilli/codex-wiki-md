<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take the linear limit and write $g_j(t)=\partial_x^jq(0,t)$. The spatial and temporal [Volterra integral equations](../../../../../../volterra-integral-equation.md) give, to first order,

$$
b(k)=-Q_0(2k),\qquad
B(k)=-\int_0^T e^{8ik^3s}[g_2(s)+2ikg_1(s)-4k^2g_0(s)]\,ds,
$$

while $a=A=1$ to first order and $c(k,T)=-\widehat q(2k,T)$. The minus sign in $b$ comes from the spatial path running from infinity to zero. For $B$, the inverse in $S=e^{4ik^3T\widehat\sigma_3}\mu_2(0,T)^{-1}$ supplies the minus sign; its conjugation cancels the final-time exponential in the temporal kernel. Substitution in the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) therefore yields

$$
e^{8ik^3T}\widehat q(2k,T)
=Q_0(2k)+4k^2G_0-2ikG_1-G_2,\qquad
G_j=\int_0^T e^{8ik^3s}g_j(s)\,ds.
$$

This is the [backward-sign Airy half-line global relation](../../../../../../backward-sign-airy-half-line-global-relation.md), because the linear limit is $q_t-q_{xxx}=0$, independently of $\lambda$.

Its constraint is especially transparent after a time [Laplace transform](../../../../../../laplace-transform.md). Let $\operatorname{Re}p>0$, choose the principal root $r=p^{1/3}$ with positive real part, and set $k=-ir/2$ in the lower transform half-plane. Then $8ik^3=-p$. Taking the infinite-horizon Laplace limit for a solution of sufficient exponential order gives

$$
\boxed{\widetilde g_2(p)=Q_0(-ir)-r\widetilde g_1(p)-r^2\widetilde g_0(p).}
$$

This proves that the second-derivative trace is fixed by the initial data and two boundary traces; it is not a third freely prescribable datum. Finite-horizon versions retain the terminal transform and express the same relation on $0<t<T$.

To see that two are necessary, rather than merely sufficient to eliminate a transform, the homogeneous transformed spatial equation is $\partial_x^3u-pu=0$. Its roots are $r$, $e^{2\pi i/3}r$, and $e^{4\pi i/3}r$. Since $-\pi/6<\arg r<\pi/6$, exactly two roots have negative real part. Decay at infinity retains two independent spatial modes. Their value/first-derivative boundary matrix has determinant equal to the difference of those two roots, which is nonzero. Thus prescribed $g_0,g_1$ fix both modes; one condition leaves a free mode, while three arbitrary traces overdetermine them.

**Two independent admissible boundary conditions are needed at $x=0$, for example $q(0,t)$ and $q_x(0,t)$.** This is the [two boundary traces for reverse-dispersion Airy flow](../../../../../../two-boundary-traces-for-reverse-dispersion-airy-flow.md) count and hence the perturbative count for the nonlinear [modified Korteweg-De Vries equation](../../../../../../modified-korteweg-de-vries-equation.md). The argument determines the small-norm boundary count; it does not claim a global nonlinear existence theorem for arbitrary large boundary data or arbitrary incompatible choices of traces.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
