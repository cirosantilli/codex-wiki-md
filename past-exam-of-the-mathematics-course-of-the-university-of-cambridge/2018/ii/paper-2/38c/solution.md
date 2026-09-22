<h1 id="38c/solution">Solution</h1>

↑ **Parent:** [38C](../38c.md)

Take $k>0$; reflection in $x$ supplies the result for negative [wavenumber](../../../../../wavenumber.md). Since each region has uniform base velocity, the perturbation is an incompressible, irrotational flow with a [velocity potential](../../../../../velocity-potential.md) satisfying the [Laplace equation](../../../../../laplace-equation.md). Its decaying outer forms are

$$
\phi_+=A_+e^{-k(y-h)}e^{ikx+\sigma t},
\qquad
\phi_-=A_-e^{k(y+h)}e^{ikx+\sigma t}.
$$

For a [varicose mode of a planar jet](../../../../../varicose-mode-of-a-planar-jet.md), reflection symmetry makes the inner potential proportional to $\cosh(ky)$; for a [sinuous mode of a planar jet](../../../../../sinuous-mode-of-a-planar-jet.md), it is proportional to $\sinh(ky)$.

At the upper interface, the linearized [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) is

$$
\sigma\eta=\partial_y\phi_+(h),
\qquad
(\sigma+ikU)\eta=\partial_y\phi_{\rm in}(h).
$$

The first equation gives $\phi_+(h)=-\sigma\eta/k$. The second gives

$$
\phi_{\rm in}(h)=\frac{\sigma+ikU}{k}\eta
\begin{cases}
\coth(kh),&\text{varicose},\\
\tanh(kh),&\text{sinuous}.
\end{cases}
$$

The linearized [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md) gives $p'=-\rho(\partial_t+U\partial_x)\phi$. Applying [pressure continuity](../../../../../pressure-continuity.md) therefore produces the [equal-density top-hat planar-jet dispersion relation](../../../../../equal-density-top-hat-planar-jet-dispersion-relation.md)

$$
\boxed{\sigma^2+F(\sigma+ikU)^2=0,}
\qquad
F=
\begin{cases}
\coth(kh),&\text{varicose},\\
\tanh(kh),&\text{sinuous}.
\end{cases}
$$

Solving the [quadratic equation](../../../../../quadratic-equation.md) gives

$$
\sigma=\frac{kU}{1+F}\left(\pm\sqrt F-iF\right).
$$

Equivalently,

$$
\boxed{
\begin{aligned}
\sigma_{\rm var}
&=\pm\frac{kU}{2}\sqrt{1-e^{-4kh}}
-\frac{ikU}{2}(1+e^{-2kh}),\\
\sigma_{\rm sin}
&=\pm\frac{kU}{2}\sqrt{1-e^{-4kh}}
-\frac{ikU}{2}(1-e^{-2kh}).
\end{aligned}}
$$

The plus sign is the unstable [Kelvin-Helmholtz instability](../../../../../kelvin-helmholtz-instability.md) branch. In particular, the two modes have exactly the same [growth rate](../../../../../growth-rate.md),

$$
\boxed{\sigma_R(k)=\frac{kU}{2}\sqrt{1-e^{-4kh}}.}
$$

Its limiting forms are

$$
\boxed{
\sigma_R\sim U\sqrt h\,k^{3/2}\quad(kh\to0),
\qquad
\sigma_R\sim\frac{Uk}{2}\quad(kh\to\infty).}
$$

Thus neither type grows faster in this equal-density idealization, although their phase speeds differ. The unbounded large-$k$ growth is the familiar short-wave pathology of an inviscid [vortex sheet](../../../../../vortex-sheet.md).

<a id="38c/image-growth-rate-of-varicose-and-sinuous-planar-jet-disturbances"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2-planar-jet-growth-rate.png)

**[Figure 3](#38c/image-growth-rate-of-varicose-and-sinuous-planar-jet-disturbances). Growth rate of varicose and sinuous planar-jet disturbances**. The two modes have the same dimensionless growth curve, with the long-wave and short-wave asymptotes shown.

## ↑ Ancestors (10)

1. [38C](../38c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
