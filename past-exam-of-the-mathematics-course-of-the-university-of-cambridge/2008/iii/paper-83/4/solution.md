<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [arc length](../../../../../arc-length.md) $s$ and the unit tangent $\mathbf t=\partial_s\mathbf r$ of an [inextensible filament](../../../../../inextensible-filament.md). In the high-force state choose its positive longitudinal branch. The constraint gives

$$
t_z=\sqrt{1-|\mathbf t_\perp|^2}=1-\frac12|\mathbf t_\perp|^2+O(|\mathbf t_\perp|^4).
$$

The extension is $z=\int_0^L t_zds=L-\frac12\int_0^L|\mathbf t_\perp|^2ds+\cdots$. The [curvature of a space curve](../../../../../curvature-of-a-space-curve.md) obeys $\kappa^2=|\partial_s\mathbf t|^2$. Since $\partial_st_z=-\mathbf t_\perp\cdot\partial_s\mathbf t_\perp+\cdots$ is second order in small fluctuations, its squared contribution is fourth order. Thus the [worm-like chain](../../../../../worm-like-chain.md) energy through quadratic order is

$$
\boxed{\mathcal E=-fL+\frac12\int_0^L\left[A|\partial_s\mathbf t_\perp|^2+f|\mathbf t_\perp|^2\right]ds.}
$$

Positive force suppresses transverse orientation fluctuations, while the [filament bending modulus](../../../../../filament-bending-modulus.md) penalizes their spatial variation.

To apply the [equipartition theorem](../../../../../equipartition-theorem.md) without missing either component or a mode-counting factor, expand each component in a real orthonormal basis of eigenfunctions of $-\partial_s^2$, $t_\alpha(s)=\sum_q a_{\alpha q}w_q(s)$, with $\int w_qw_{q'}ds=\delta_{qq'}$ and $\alpha=x,y$. The quadratic energy is $\frac12\sum_{\alpha,q}(Aq^2+f)a_{\alpha q}^2$. Each real quadratic degree of freedom contributes $k_BT/2$, so

$$
\langle a_{\alpha q}a_{\beta q'}\rangle=\frac{k_BT}{Aq^2+f}\delta_{\alpha\beta}\delta_{qq'}.
$$

For a chain long compared with the force-dependent [correlation length](../../../../../correlation-length.md), the interior is translation invariant and the mode sum per length becomes $\int dq/(2\pi)$. Equivalently, for the [Fourier transform](../../../../../fourier-transform.md) $\widetilde t_\alpha(q)=\int e^{-iqs}t_\alpha(s)ds$,

$$
\langle\widetilde t_\alpha(q)\widetilde t_\beta(q')\rangle=2\pi\delta(q+q')\delta_{\alpha\beta}\frac{k_BT}{Aq^2+f}.
$$

The negative and positive wavenumbers here represent the real-field mode count consistently, rather than two independent complex modes. Summing both transverse components gives the [high-force worm-like chain elasticity](../../../../../high-force-worm-like-chain-elasticity.md)

$$
\langle|\mathbf t_\perp|^2\rangle=2k_BT\int_{-\infty}^{\infty}\frac{dq}{2\pi}\frac1{Aq^2+f}=\frac{k_BT}{\sqrt{Af}},
$$

where the integral follows by setting $q=\sqrt{f/A}\,u$ and using $\int_{-\infty}^{\infty}(1+u^2)^{-1}du=\pi$. Therefore

$$
\boxed{\frac{\langle z\rangle}{L}=1-\frac{k_BT}{2\sqrt{Af}}=1-\sqrt{\frac{k_BT}{4L_pf}},\qquad L_p=\frac{A}{k_BT}.}
$$

Here $L_p$ is the three-dimensional zero-force [persistence length](../../../../../persistence-length.md). The result requires $fL_p\gg k_BT$, negligible backbone stretching, and a long-chain bulk approximation. It does not describe the eventual bond-stretching regime. For a continuum polymer description, the force-dependent length should also exceed the microscopic cutoff.

For comparison, a three-dimensional [freely jointed chain](../../../../../ideal-chain.md) has contour length $L=Nb$ and independent link orientations. At force $f$, a link of polar angle $\vartheta$ has Boltzmann factor $e^{x\cos\vartheta}$ with $x=fb/(k_BT)$. Its angular [canonical partition function](../../../../../canonical-partition-function.md) is

$$
Z_1=2\pi\int_{-1}^1e^{xu}du=4\pi\frac{\sinh x}{x}.
$$

The total [canonical partition function](../../../../../canonical-partition-function.md) is $Z_1^N$. Differentiating with respect to force gives the [force-extension of a three-dimensional freely jointed chain](../../../../../force-extension-of-a-three-dimensional-freely-jointed-chain.md):

$$
\frac{\langle z\rangle}{Nb}=\frac{d\log Z_1}{dx}=\coth x-\frac1x.
$$

Consequently

$$
\boxed{1-\frac{\langle z\rangle}{L}\sim\frac{k_BT}{fb}\quad\text{for a freely jointed chain},\qquad 1-\frac{\langle z\rangle}{L}\sim\frac{k_BT}{2\sqrt{Af}}\quad\text{for a worm-like chain}.}
$$

The extension deficits scale as $f^{-1}$ and $f^{-1/2}$ respectively. Inverting them gives force divergences proportional to the first and second inverse powers of the deficit. Freely jointed link rotations cost no bending energy; the [worm-like chain](../../../../../worm-like-chain.md) instead has a continuum of coupled bending modes whose contributing wavelengths change with force. Setting a long-wavelength coarse-grained link length $b=2L_p$ can match weak-force statistics, but does not make these high-force laws identical.

For the [transverse tangent correlation of a stretched worm-like chain](../../../../../transverse-tangent-correlation-of-a-stretched-worm-like-chain.md), use a separation $r$ consistently: the source writes $C(y)$ but integrates a separation denoted $r$. In the translation-invariant bulk the spatial average is redundant and

$$
C(r)=\langle\mathbf t_\perp(s)\cdot\mathbf t_\perp(s+r)\rangle=2k_BT\int_{-\infty}^{\infty}\frac{dq}{2\pi}\frac{e^{iqr}}{Aq^2+f}.
$$

To evaluate the integral without an assumed decay law, let $G(r)$ be the inverse [Fourier transform](../../../../../fourier-transform.md) of $(Aq^2+f)^{-1}$. Then $(-A\partial_r^2+f)G=\delta(r)$. Away from zero, decay at both infinities requires $G=B e^{-|r|/\xi}$ with $\xi=\sqrt{A/f}$. Integrating across zero yields $-A[G'(0^+)-G'(0^-)]=1$, so $B=1/(2\sqrt{Af})$. Thus

$$
\boxed{C(r)=\frac{k_BT}{\sqrt{Af}}e^{-|r|/\xi},\qquad\xi=\sqrt{\frac Af}=\sqrt{\frac{k_BT L_p}{f}}.}
$$

At $r=0$ this agrees with the two-component [equipartition theorem](../../../../../equipartition-theorem.md) calculation. The [correlation length](../../../../../correlation-length.md) decreases with force and is distinct from the zero-force [persistence length](../../../../../persistence-length.md). The full tangent correlation has a nonzero aligned background; the exponentially decaying quantity here is specifically the transverse correlation.

For a finite open chain, the source's integral samples $s+r$ beyond $L$ and supplies no endpoint tangent conditions. An exact finite-length correlation is therefore not uniquely specified. The result above is the intended bulk form when $L\gg\xi$. As one explicit finite convention, periodically extending the tangent fluctuations gives the [periodic finite-length tangent correlation of a stretched worm-like chain](../../../../../periodic-finite-length-tangent-correlation-of-a-stretched-worm-like-chain.md)

$$
C_L(r)=\sum_{j\in\mathbb Z}C(r+jL)=\frac{k_BT}{\sqrt{Af}}\frac{\cosh[(L/2-d_L(r))/\xi]}{\sinh[L/(2\xi)]},
$$

where $d_L(r)$ is the distance from zero around the periodic interval. Then $C_L(0)=(k_BT/\sqrt{Af})\coth[L/(2\xi)]$, and the extension formula acquires this same finite-length factor. The bulk law is recovered as $L/\xi\to\infty$. This makes the endpoint assumption explicit rather than claiming an unspecified finite-chain correlation is exactly translationally invariant.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
