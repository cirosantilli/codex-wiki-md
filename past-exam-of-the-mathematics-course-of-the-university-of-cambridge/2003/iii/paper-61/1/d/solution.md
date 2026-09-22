<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For asymptotic analysis it is useful to separate the spectral density from the observation time. For a fixed horizon $T\ge t$, $H(k,T)$ already has this property. If the boundary traces extend to all positive times with suitable growth, their one-sided [Laplace transforms](../../../../../../laplace-transform.md) give the infinite-horizon version

$$
G_j^\infty(k)=\int_0^\infty e^{w(k)s}g_j(s)\,ds
=\mathcal Lg_j(-w(k)),\qquad
H_\infty=-Q_0(\nu)+(k^2-\nu^2)\mathcal Lg_0(-w)-i(k-\nu)\mathcal Lg_1(-w).
$$

For bounded traces these integrals converge in $D_+$; boundary values are taken by an Abel limit where needed. The finite-horizon formula permits this replacement: the tail from $t$ to infinity contributes an analytic, decaying integrand with zero integral around $\partial D_+$. **The resulting spectral functions are independent of $t$.**

They can be made particularly explicit on the two contour pieces. On the real axis and upper curve, respectively,

$$
\nu_{\mathbb R}(k)=-\frac k2-\frac i2\sqrt{3k^2+4},\qquad
\nu_C(k)=\overline k.
$$

The second identity follows because $k^3+k$ is real on $C$: the remaining roots are $\overline k$ and $-2\operatorname{Re}k$. Therefore rewrite the solution as

$$
q=\frac1{2\pi}\int_{\mathbb R}e^{ikx-i(k+k^3)t}[Q_0(k)+H_{\infty,\mathbb R}(k)]\,dk
+\frac1{2\pi}\int_Ce^{ikx-i(k+k^3)t}H_{\infty,C}(k)\,dk.
$$

This isolates all large-time dependence in the exponential, allowing the [stationary phase method](../../../../../../stationary-phase-method.md) or the [method of steepest descent](../../../../../../method-of-steepest-descent.md). Along $x/t=\xi$, the phase is $i[k\xi-k-k^3]$, and its [stationary points](../../../../../../stationary-point.md) satisfy $3k^2=\xi-1$. Thus the real saddles coalesce at $\xi=1$; any poles arising from the boundary [Laplace transforms](../../../../../../laplace-transform.md) also have to be retained during contour deformation.

The source specifies smooth boundary traces, not their large-time decay or growth. Accordingly a universal numerical long-time profile cannot be inferred. The infinite-horizon formula requires the stated additional transform hypothesis; for more general data the finite-horizon density $H(k,T)$ remains valid, or an appropriately shifted Laplace contour must be used. This qualification does not leave an unknown boundary trace in the representation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
