<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\omega(k)=k^2-i\alpha k$ and $\nu(k)=i\alpha-k$, so $\omega(\nu)=\omega(k)$. For boundary traces $h_j(s)=\partial_x^jq(0,s)$, define

$$
Q(k)=\int_0^\infty e^{-ikx}q_0(x)dx,\qquad G_j(k,t)=\int_0^t e^{\omega(k)s}h_j(s)ds.
$$

The [Half-range Fourier transform](../../../../../../half-range-fourier-transform.md) of the equation is obtained by two integrations by parts:

$$
\partial_t\widehat q=-\omega(k)\widehat q-h_1(t)-(ik+\alpha)h_0(t).
$$

Solving this scalar equation gives the [drift-diffusion half-line global relation](../../../../../../drift-diffusion-half-line-global-relation.md)

$$
e^{\omega(k)t}\widehat q(k,t)=Q(k)-G_1(k,t)-(ik+\alpha)G_0(k,t),\qquad\operatorname{Im}k\leq0.
$$

In particular the reflected relation is valid on $L$, since $\operatorname{Im}\nu(k)\leq0$ there.

In the region between the real axis and $L$, $\operatorname{Re}\omega\geq0$. Thus a boundary contribution $e^{-\omega t}G_j=\int_0^t e^{-\omega(t-s)}h_j(s)ds$ admits an upward [contour deformation](../../../../../../contour-deformation.md) from the real axis to $L$. Large-contour estimates follow from the spatial exponential and the time integral; at the upper time endpoint one can integrate in time once or use a small contour displacement. The initial-data transform is retained on the real axis. Hence, if $I_C[F]=(2\pi)^{-1}\int_C e^{ikx-\omega(k)t}F(k)dk$, ordinary inversion first gives

$$
q=I_{\mathbb R}[Q]-I_L[G_1+(ik+\alpha)G_0].
$$

For the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md), take $h_0=g_0$. Subtract the null integral of the reflected time-dependent transform, using the inversion from part (a) with $c=-1$. The unknown derivative transform cancels because $i\nu+\alpha=-ik$. This derives the [Dirichlet spectral formula for half-line constant drift](../../../../../../dirichlet-spectral-formula-for-half-line-constant-drift.md):

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega(k)t}Q(k)dk-\frac1{2\pi}\int_L e^{ikx-\omega(k)t}\left[Q(\nu(k))+(2ik+\alpha)G_0(k,t)\right]dk.}
$$

Only initial and prescribed boundary data occur in this expression.

For the [Neumann boundary condition](../../../../../../neumann-boundary-condition.md), take $h_1=g_1$. The reflected [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) reads $e^{\omega t}\widehat q(\nu,t)=Q(\nu)-G_1+ikG_0$. Solve for $G_0$ and substitute it in the preliminary representation. The leftover term is a null integral with multiplier $(ik+\alpha)/(ik)$, analytic above $L$; its pole at zero is below the contour. Thus the [Neumann spectral formula for half-line constant drift](../../../../../../neumann-spectral-formula-for-half-line-constant-drift.md) is

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega(k)t}Q(k)dk+\frac1{2\pi}\int_L e^{ikx-\omega(k)t}\left[\frac{ik+\alpha}{ik}Q(\nu(k))-\frac{2ik+\alpha}{ik}G_1(k,t)\right]dk.}
$$

There is no residue from the origin, since this elimination never moves the contour across it. The given derivative is the inward-coordinate derivative $q_x$, not the outward derivative $-q_x$. The initial compatibility for this case is $q_0'(0)=g_1(0)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
