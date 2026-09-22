<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write the base-state gradients as

$$
G_w=\frac{T_h-T_m}{h},
\qquad
G_a=\frac{T_a-T_h}{\delta}.
$$

The base [heat flux](../../../../../../heat-flux-density.md) and [Stefan condition](../../../../../../stefan-condition.md) relations are

$$
k_wG_w=k_aG_a,
\qquad
-k_wG_w=\rho_iL_fV.
$$

Under the [quasi-stationary approximation](../../../../../../quasi-steady-approximation.md), and with advective heat transport neglected, each temperature perturbation satisfies the [Laplace equation](../../../../../../laplace-equation.md). The decaying normal-mode solutions are

$$
\widehat T_w=A\cosh(\alpha x)+B\sinh(\alpha x),
\qquad
\widehat T_a=Ce^{-\alpha(x-h)}.
$$

Keeping the displaced ice interface at $T_m$ omits the curvature correction described by the [Gibbs--Thomson relation](../../../../../../gibbs-thomson-relation.md).  
The fixed melting temperature at the displaced ice interface gives

$$
A=-\eta_1G_w.
$$

Expanding temperature and conductive [heat flux](../../../../../../heat-flux-density.md) continuity at the displaced outer interface gives

$$
A\cosh(\alpha h)+B\sinh(\alpha h)-C
=\eta_2(G_a-G_w),
$$



$$
k_w\left[A\sinh(\alpha h)+B\cosh(\alpha h)\right]
=-k_aC.
$$

Put $r=k_a/k_w$. Since $G_a=G_w/r$, the temperature condition in the limits $r\ll1$ and $\alpha h\ll1$ gives

$$
C\sim-\frac{\eta_2G_w}{r}.
$$

Although $r$ is small, the product $rC$ is therefore order one and cannot be discarded. The flux condition then gives

$$
B=-rC-A\alpha h+o(1)
\sim\eta_2G_w.
$$

This is why the stated asymptotic warning matters.

The perturbed [Stefan condition](../../../../../../stefan-condition.md) at $x=0$ is

$$
\rho_iL_f\sigma\eta_1
=-k_w\widehat T_w'(0)
=-k_w\alpha B.
$$

Using $B\sim\eta_2G_w$ and $-k_wG_w=\rho_iL_fV$ yields

$$
\sigma\eta_1=V\alpha\eta_2.
$$

Substitution of the interface-amplitude ratio from part i produces the [thin-film icicle-ripple instability](../../../../../../thin-film-icicle-ripple-instability.md) [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{
\frac{h\sigma}{V}
=\frac{\alpha h}{1-i\Gamma\alpha^3h}}.
$$

Set $b=\Gamma h\alpha^3$. Rationalizing this [complex number](../../../../../../complex-number.md) gives

$$
\sigma=\frac{V\alpha(1+ib)}{1+b^2},
$$

so its [growth rate](../../../../../../growth-rate.md) and [imaginary part](../../../../../../imaginary-part.md) are

$$
\operatorname{Re}\sigma
=\frac{V\alpha}{1+(\Gamma h)^2\alpha^6},
\qquad
\operatorname{Im}\sigma
=\frac{V\alpha b}{1+b^2}.
$$

Differentiating the growth rate with respect to the [wavenumber](../../../../../../wavenumber.md) shows that its positive [stationary point](../../../../../../stationary-point.md) satisfies

$$
1-5(\Gamma h)^2\alpha_m^6=0.
$$

It is the unique [global maximum](../../../../../../global-maximum.md), and hence

$$
\boxed{
\alpha_m=5^{-1/6}(\Gamma h)^{-1/3}}.
$$

At this wavenumber $b=1/\sqrt5$. With the convention $e^{i\alpha z+\sigma t}$, a constant phase travels with [phase velocity](../../../../../../phase-velocity.md)

$$
c_p=-\frac{\operatorname{Im}\sigma}{\alpha}
=-\frac{Vb}{1+b^2}.
$$

Therefore

$$
\boxed{c_p=-\frac{\sqrt5}{6}V}.
$$

Because $z$ increases downward, the negative sign means that the [icicle ripples](../../../../../../icicle-ripple.md) migrate upward with speed $\sqrt5V/6$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
