<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The original PDF has a spatial shift $u_{m+2}^{n+2}$, so the printed scheme is not the usual second-order BDF discretization.** The PDF does have $-2u_m^{n+2}$ on the right; the TeX aid loses that factor two, and that transcription must not be used.

Let $h=\Delta x$, $k=\Delta t$, and expand an exact smooth [heat equation](../../../../../../heat-equation.md) solution about $(x_m,t_{n+2})$. Relative to the standard unshifted [backward differentiation formula](../../../../../../backward-differentiation-formula.md), the printed newest value adds

$$
u(x_m+2h,t)-u(x_m,t)=2hu_x+2h^2u_{xx}+O(h^3).
$$

Dividing the raw residual by $2k/3$, its expansion is

$$
u_t-u_{xx}+\frac{3h}{k}u_x+\frac{3h^2}{k}u_{xx}
-\frac{k^2}{3}u_{ttt}-\frac{h^2}{12}u_{xxxx}
+O(k^3+h^4+h^3/k).
$$

In particular, for the usual refinement $k=\mu h^2$ with fixed $\mu>0$, the term $3u_x/(\mu h)$ generally diverges. A concrete smooth counterexample is $u=e^{-\pi^2t/4}\cos(\pi x/2)$, which satisfies the [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) and has $u_x\ne0$ at $x=1/2$. Thus **the printed scheme has no consistent order under fixed-$\mu$ refinement**. Its normalized shift error is $O(h/k)$, so one could only investigate a special coupled limit such as $h=o(k)$ after specifying a valid boundary closure; it has no standard joint second-order accuracy.

For the likely intended correction $u_m^{n+2}$, the extra shift terms disappear. The normalized [local truncation error](../../../../../../local-truncation-error.md) is

$$
-\frac{k^2}{3}u_{ttt}-\frac{h^2}{12}u_{xxxx}+O(k^3+h^4).
$$

With a stable, suitably accurate starter, the corrected [backward differentiation formula](../../../../../../backward-differentiation-formula.md) combined with the [second-order central difference](../../../../../../second-order-central-difference.md) therefore has

$$
\boxed{\text{order two in time and order two in space}}.
$$

This is a correction to the printed method, not a claim about it.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
