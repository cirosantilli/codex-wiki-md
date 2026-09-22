<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $e_{ij}=(\partial_i u_j+\partial_j u_i)/2$ be the [rate-of-strain tensor](../../../../../strain-rate-tensor.md) of an [incompressible flow](../../../../../incompressible-flow.md), and let $s(t)$ be the supremum over the conductor of its largest [eigenvalue](../../../../../eigenvalue.md). State [Backus' necessary condition for dynamo action](../../../../../backus-necessary-condition-for-dynamo-action.md) with its magnetic boundary conditions: an isolated bounded conductor of uniform positive [magnetic diffusivity](../../../../../magnetic-diffusivity.md) $\eta$, surrounded by an electrical insulator with a decaying potential exterior field, and no imposed magnetic field or boundary energy input. For definiteness take a [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) on the fluid, which eliminates the stretching surface term. If the conductor lies within a sphere of radius $R$ and $S=\sup_t s(t)$, **a necessary condition for a nondecaying dynamo is**

$$
\boxed{S\geq\frac{\eta\pi^2}{R^2},\qquad\operatorname{Rm}_{\rm strain}=\frac{SR^2}{\eta}\geq\pi^2.}
$$

The constant is the free-decay spectral bound for an insulating exterior, not a universal constant for every magnetic boundary condition. The condition is necessary, not sufficient, and involves maximum stretching rather than an rms velocity.

To see both the condition and the growth-rate bound, include exterior [magnetic energy](../../../../../magnetic-energy.md):

$$
E_B=\frac1{2\mu_0}\int_{\mathbb R^3}|\mathbf B|^2\,dV,
\qquad
\frac{dE_B}{dt}=\frac1{\mu_0}\int_D B_i e_{ij}B_j\,dV
-\frac\eta{\mu_0}\int_D|\nabla\times\mathbf B|^2\,dV.
$$

This follows from the [resistive induction equation](../../../../../resistive-induction-equation.md) and [integration by parts](../../../../../integration-by-parts.md), with the stated boundary assumptions. The [magnetic free-decay spectral bound](../../../../../magnetic-free-decay-spectral-bound.md) is $\int_D|\nabla\times\mathbf B|^2\,dV\geq(\pi^2/R^2)\int_{\mathbb R^3}|\mathbf B|^2\,dV$. For a sphere its lowest mode is the dipolar poloidal free-decay mode; enclosing a smaller conductor gives the same valid lower bound. Since $B_i e_{ij}B_j\leq s(t)|\mathbf B|^2$, we obtain

$$
\frac{dE_B}{dt}\leq2\left[s(t)-\frac{\eta\pi^2}{R^2}\right]E_B.
$$

Integrating this differential inequality gives decay whenever $S<\eta\pi^2/R^2$. More generally the exponential rate of the field norm, rather than of its squared energy, satisfies

$$
\boxed{g_B=\limsup_{t\to\infty}\frac1{2t}\log\frac{E_B(t)}{E_B(0)}
\leq\limsup_{t\to\infty}\frac1t\int_0^t s(\tau)\,d\tau-\frac{\eta\pi^2}{R^2}\leq S.}
$$

Simply discarding the nonnegative resistive dissipation already proves the requested maximum-strain bound. The energy exponent is twice the field-amplitude exponent.

For the [alpha-Omega dynamo](../../../../../alpha-omega-dynamo.md) model, write $a=|\alpha_0|$, $w=|\Omega|$, $k\geq0$ and $d=\eta k^2$. Direct differentiation gives

$$
\begin{aligned}
\frac d{dt}|A|^2&=2\operatorname{Re}(\alpha_0 fB\overline A)-2d|A|^2
\leq2a|A||B|-2d|A|^2,\\
\frac d{dt}|B|^2&=2\operatorname{Re}(ik\Omega A\overline B)-2d|B|^2
\leq2kw|A||B|-2d|B|^2.
\end{aligned}
$$

For $a,kw>0$, use the [weighted energy estimate for two coupled modes](../../../../../weighted-energy-estimate-for-two-coupled-modes.md) and form the positive weighted norm $N=kw|A|^2+a|B|^2$. The inequality $N\geq2\sqrt{akw}|A||B|$ gives

$$
\dot N\leq4akw|A||B|-2dN
\leq2(\sqrt{akw}-\eta k^2)N.
$$

For each fixed $k$ and model parameters, this norm is equivalent to the amplitude norm; its square-root exponential rate is therefore bounded by $h(k)=\sqrt{awk}-\eta k^2$, uniformly over all admissible $f(t)$. Maximizing over $k$ gives

$$
k_*=\left(\frac{aw}{16\eta^2}\right)^{1/3},\qquad
\boxed{g_{\max}\leq\frac3{2^{8/3}}\left(\frac{a^2w^2}{\eta}\right)^{1/3}.}
$$

The exponent is also achievable in order of magnitude. Choose the admissible constant $f=1$. The growing [eigenvalue](../../../../../eigenvalue.md) of the two-component system has real part $-\eta k^2+\sqrt{awk/2}$. Its maximum occurs at $k=(aw/(32\eta^2))^{1/3}$ and equals $3\,2^{-10/3}(a^2w^2/\eta)^{1/3}$. Thus **the [bounded-modulation alpha-Omega growth estimate](../../../../../bounded-modulation-alpha-omega-growth-estimate.md) has the scaling**

$$
\boxed{g_{\max}=\Theta\!\left(|\alpha_0|^{2/3}|\Omega|^{2/3}\eta^{-1/3}\right)
\quad\text{for fixed nonzero }\alpha_0,\eta\text{ as }|\Omega|\to\infty.}
$$

This means the maximum over allowed modulations and wavenumbers, not that every bounded modulation grows; $f=0$ supplies no regenerating alpha coupling.

The [Omega effect](../../../../../omega-effect.md) rapidly makes toroidal field from poloidal field, but exponential [dynamo action](../../../../../dynamo-action.md) also requires the slower [alpha effect](../../../../../alpha-effect.md) to regenerate the poloidal component. The coupled amplification rate is of order $\sqrt{a\Omega k}$ rather than $\Omega$; shortening the wavelength to increase it also increases [magnetic diffusion](../../../../../magnetic-diffusion.md) as $\eta k^2$. Their optimal balance gives $k\sim\Omega^{1/3}$ and growth $\sim\Omega^{2/3}$. The [Backus' necessary condition for dynamo action](../../../../../backus-necessary-condition-for-dynamo-action.md) estimate controls stretching alone and does not incorporate this regeneration bottleneck. A shear without regeneration can give transient amplification but not this sustained exponential feedback.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
