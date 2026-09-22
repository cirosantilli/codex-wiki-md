<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [Bromwich inversion formula](../../../../../../bromwich-inversion-formula.md) in the real variable $\omega$, with $p=\gamma+i\omega$:

$$
u(x,t)=\frac{e^{-ax+\gamma t}}{2\pi}\int_{-\infty}^{\infty}e^{i\omega t}W(x,\gamma+i\omega)\,d\omega.
$$

When the relevant [Laplace transforms](../../../../../../laplace-transform.md) and spatial [integral transforms](../../../../../../integral-transform.md) are explicit, every sample of this integrand can be evaluated directly, without a time-stepping approximation to the [partial differential equation](../../../../../../partial-differential-equation-split.md). Split the [initial condition](../../../../../../initial-condition.md) integral at $y=x$: the two pieces of $R_q$ are linear combinations of $e^{\pm qy}$, so truncated spatial exponential transforms suffice. For real data the negative-frequency half is the [complex conjugate](../../../../../../complex-conjugate.md) of the positive-frequency half.

A practical [numerical integration](../../../../../../numerical-integration.md) is to truncate to $|\omega|\leq\Omega$, apply an adaptive [quadrature rule](../../../../../../quadrature-rule.md), and independently increase $\Omega$ and refine the quadrature. Choose $\gamma>0$ large enough to remain to the right of all singularities, but avoid an unnecessarily large $e^{\gamma t}$. Evaluate [hyperbolic function](../../../../../../hyperbolic-function.md) ratios in scaled form; for example,

$$
\frac{\sinh(q[L-x])}{\sinh(qL)}=e^{-qx}\frac{1-e^{-2q(L-x)}}{1-e^{-2qL}}.
$$

This prevents overflow when $\operatorname{Re}qL$ is large. The boundary contributions at an interior point are damped by $e^{-x\operatorname{Re}q}$ or $e^{-(L-x)\operatorname{Re}q}$, with $\operatorname{Re}q\sim\sqrt{|\omega|/2}$. Near an endpoint more frequencies are needed; at the endpoint itself use the prescribed [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md). The [initial condition](../../../../../../initial-condition.md) resolvent has a generally only $O(1/\omega)$ tail. Treat its oscillatory tail accurately, subtract a known transform with the same leading term, or evaluate that contribution separately with the [heat kernel](../../../../../../heat-kernel.md).

An equally useful check is the [eigenfunction expansion](../../../../../../eigenfunction-expansion.md). Define

$$
U_n=\frac2L\int_0^Le^{ay}u_0(y)\sin(q_ny)\,dy,\qquad \lambda_n=q_n^2+a^2.
$$

The causal modal formula is

$$
u(x,t)=e^{-ax}\sum_{n=1}^{\infty}\sin(q_nx)\left[e^{-\lambda_nt}U_n+\frac{2q_n}{L}\int_0^te^{-\lambda_n(t-s)}\left(g_0(s)-(-1)^ne^{aL}h(s)\right)ds\right].
$$

It follows either from the [heat kernel](../../../../../../heat-kernel.md) formula or directly from [integration by parts](../../../../../../integration-by-parts.md) against a sine [eigenfunction](../../../../../../eigenfunction.md). Exponential-transform formulas evaluate the time [integral](../../../../../../integral.md) explicitly when available. The [initial condition](../../../../../../initial-condition.md) contribution has a [Gaussian function](../../../../../../gaussian-function.md) cutoff in $n$ for each positive time. Nonzero endpoint forcing produces a more slowly convergent [sine series](../../../../../../fourier-sine-series.md) tail. A [boundary lifting](../../../../../../boundary-lifting.md) $\ell(x,t)=(1-x/L)g_0(t)+(x/L)e^{aL}h(t)$ gives $w=\ell+z$, where $z$ has zero [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) and forcing $-\ell_t-a^2\ell$; expanding $z$ gives better convergence and imposes the endpoint values exactly. At very small times the [method of images](../../../../../../method-of-images.md) is often more efficient than retaining many modes.

**Check convergence by increasing both the frequency cutoff and quadrature resolution, and compare with a separately truncated causal modal or image-kernel evaluation.** [Causality in finite-time Laplace contour inversion](../../../../../../causality-in-finite-time-laplace-contour-inversion.md) means a leftward contour deformation must respect both [resolvent operator](../../../../../../resolvent-of-an-operator.md) poles and growth of the transformed data. In particular, the transform of data extended by zero after $T$ can grow like $e^{-pT}$ in the left half-plane: for $t<T$ one cannot close that contour indiscriminately and discard its large arc. The modal forcing integral with upper limit $t$ avoids this causality error.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 328](../../../paper-328-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
