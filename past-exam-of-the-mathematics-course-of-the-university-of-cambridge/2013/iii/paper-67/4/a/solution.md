<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substitution of a [normal mode](../../../../../../normal-mode.md) gives the [dispersion relation](../../../../../../dispersion-relation.md)

$$
D(k,\omega)=-i\omega-\alpha k^2+\beta k^4+\gamma=0,\qquad
\omega=i\sigma(k),\quad \sigma(k)=\alpha k^2-\beta k^4-\gamma.
$$

For real $k$, $\sigma$ is the temporal growth rate. Since $\beta\ne0$, its supremum is finite exactly when

$$
\boxed{\beta>0}.
$$

For $\beta<0$, arbitrarily short wavelengths grow arbitrarily fast. For $\beta>0$, the [finite maximum temporal growth rate](../../../../../../finite-maximum-temporal-growth-rate.md) is

$$
\sigma_{\max}=\begin{cases}\alpha^2/(4\beta)-\gamma,&\alpha>0,\\-\gamma,&\alpha<0.\end{cases}
$$

The [Briggs-Bers criterion](../../../../../../briggs-bers-criterion.md) starts the inverse temporal [Laplace transform](../../../../../../laplace-transform.md) above all temporal singularities and then deforms its contour downward while following the spatial roots. A finite growth bound supplies such an initial contour and a causal, high-frequency-controlled [Green function](../../../../../../green-s-function.md). Unbounded temporal growth prevents that standard construction.

For [absolute wave-packet instability](../../../../../../absolute-wave-packet-instability.md), a candidate [spatial pinch point](../../../../../../spatial-pinch-point.md) must satisfy $D=0$, $D_k=0$, and $\operatorname{Im}\omega>0$. Here

$$
D_k=-2\alpha k+4\beta k^3=0
$$

gives

$$
k_0=0,\quad \omega_0=-i\gamma;\qquad
k_\pm=\pm\sqrt{\frac\alpha{2\beta}},\quad
\omega_\pm=i\left(\frac{\alpha^2}{4\beta}-\gamma\right).
$$

Thus candidate growing saddles require $\gamma<0$ at $k_0$, or $\gamma<\alpha^2/(4\beta)$ at $k_\pm$. Together with $\beta>0$, existence of at least one such candidate requires $\gamma<\alpha^2/(4\beta)$.

**A growing double root is not sufficient: the roots must pinch the spatial inversion contour from opposite sides.** Collisions of branches originating in the same spatial half-plane do not obstruct the relevant deformation. This distinction is part of the [Briggs-Bers criterion](../../../../../../briggs-bers-criterion.md); it is stated, for example, in the primary study [https://doi.org/10.1017/jfm.2016.195.](https://doi.org/10.1017/jfm.2016.195.)

An explicit [false spatial saddle in quartic dispersion](../../../../../../false-spatial-saddle-in-quartic-dispersion.md) is $\alpha=-2$, $\beta=1$, $\gamma=1/2$. Its candidates $k=\pm i$ have $\omega=i/2$, but all real modes have $\sigma=-k^4-2k^2-1/2<0$. Each imaginary collision joins two branches in the same half-plane; neither is a relevant pinch. For $\omega=i\Omega$, the spatial roots obey $k^2=-1\pm\sqrt{1/2-\Omega}$, making those same-half-plane collisions transparent as $\Omega\downarrow1/2$.

For this particular real, even dispersion relation one can also establish the actual threshold directly. At the origin its impulse [Green function](../../../../../../green-s-function.md) is

$$
G(0,t)=\frac1{2\pi}\int_{-\infty}^{\infty}e^{t\sigma(k)}dk.
$$

[Laplace method](../../../../../../laplace-s-method.md) selects the real maximum, and gives a positive prefactor times $t^{-1/2}e^{\sigma_{\max}t}$ because $\alpha\ne0$. Therefore the actual [absolute wave-packet instability](../../../../../../absolute-wave-packet-instability.md) condition is

$$
\boxed{\beta>0,\quad\begin{cases}\gamma<\alpha^2/(4\beta),&\alpha>0,\\\gamma<0,&\alpha<0.\end{cases}}
$$

These are sufficient for this model as well as necessary. They follow after identifying relevant real saddles; the earlier algebraic double-root test alone lacks the pinch information. Equality is marginal, not exponential absolute growth.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
