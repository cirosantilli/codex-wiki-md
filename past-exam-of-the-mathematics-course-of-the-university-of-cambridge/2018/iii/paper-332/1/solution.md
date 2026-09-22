<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $x$ in the injection direction and $y$ along the flat interface. The specified $U$ must be a [Darcy velocity](../../../../../darcy-velocity.md), so the pore-fluid velocity and unperturbed interface speed are $U/\phi$. Write the perturbed interface as $x=X(t)+\eta(y,t)$, with $\dot X=U/\phi$, and choose the normal from fluid 1 into fluid 2. The background pressure gradients from [Darcy law](../../../../../darcy-law.md) are $\partial_xp_i^{(0)}=-\mu_iU/k$.

By [incompressibility](../../../../../incompressible-flow.md) and uniform [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md), pressure perturbations are [harmonic functions](../../../../../harmonic-function.md). A transverse [Fourier mode](../../../../../fourier-mode.md) with positive [wavenumber](../../../../../wavenumber.md) $\alpha$ has the decaying forms

$$
p_1'=A_1(t)e^{\alpha(x-X)}e^{i\alpha y},\qquad
p_2'=A_2(t)e^{-\alpha(x-X)}e^{i\alpha y},\qquad
\eta=a(t)e^{i\alpha y}.
$$

The [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) and equal normal [Darcy flux](../../../../../darcy-velocity.md) imply

$$
\phi\dot a=-\frac{k\alpha}{\mu_1}A_1=\frac{k\alpha}{\mu_2}A_2,
\qquad A_1-A_2=-\frac{\phi(\mu_1+\mu_2)}{k\alpha}\dot a.
$$

Without capillarity the pressure is continuous at the displaced interface. Its linear perturbation is therefore

$$
A_1-A_2+\frac{(\mu_2-\mu_1)U}{k}a=0.
$$

Consequently the [planar viscous-fingering dispersion relation](../../../../../planar-viscous-fingering-dispersion-relation.md) reduces to

$$
\boxed{\dot a=\sigma a,\qquad\sigma=\frac{\alpha U}{\phi}\frac{\mu_2-\mu_1}{\mu_2+\mu_1}=\frac{\alpha U}{\phi}M>0}.
$$

This is the [Saffman–Taylor instability](../../../../../saffman-taylor-instability.md): less viscous fluid advances preferentially through protrusions. Without a short-wave regularizing mechanism the idealized rate has no finite maximum.

For the prescribed apparent [capillary pressure](../../../../../capillary-pressure.md), the chosen normal is $\mathbf n=(1,-\eta_y)/\sqrt{1+\eta_y^2}$, so $\nabla\cdot\mathbf n=-\eta_{yy}+O(\eta^2)=\alpha^2\eta+O(\eta^2)$. Subtract the flat-front pressure jump $\gamma(1+\beta X)\kappa_0$. Linearization of the jump at $x=X+\eta$ gives

$$
A_1-A_2+\frac{(\mu_2-\mu_1)U}{k}a
=\gamma\bigl[\beta\kappa_0+(1+\beta X)\alpha^2\bigr]a.
$$

There is no first-order product of the surface-tension perturbation and the perturbed macroscopic [curvature](../../../../../curvature.md). Thus

$$
\boxed{\sigma(\alpha;X)=\frac{\alpha}{\phi(\mu_1+\mu_2)}
\left[(\mu_2-\mu_1)U-k\gamma\beta\kappa_0-k\gamma(1+\beta X)\alpha^2\right]}.
$$

Using the [capillary number](../../../../../capillary-number.md) convention $\mathrm{Ca}=\mu_2U/\gamma$ and $\mu_2/(\mu_1+\mu_2)=(1+M)/2$, this is

$$
\boxed{\sigma(\alpha;X)=\frac{\alpha U}{\phi}\left[M-\frac{k(1+M)}{2\mathrm{Ca}}\bigl(\beta\kappa_0+(1+\beta X)\alpha^2\bigr)\right]}.
$$

If $x$ is measured from the unperturbed front and $\gamma$ denotes its local apparent tension, set $X=0$ to obtain the usual fixed-coefficient expression. For a physically fixed spatial gradient, $X=Ut/\phi$ and the displayed rate is an instantaneous, generally time-dependent [growth rate](../../../../../growth-rate.md); the amplitude solves $\dot a=\sigma(\alpha;X(t))a$, rather than one constant exponential law for the entire displacement. The parameter $\beta$ has dimensions of inverse length; the absolute tension gradient is $\gamma\beta$.

Assume $1+\beta X>0$, as required for positive apparent [surface tension](../../../../../surface-tension.md), and define $A=(\mu_2-\mu_1)U-k\gamma\beta\kappa_0$. If $A>0$, unstable modes satisfy $0<\alpha^2<A/[k\gamma(1+\beta X)]$. Differentiating the cubic [dispersion relation](../../../../../dispersion-relation.md) gives the fastest-growing mode

$$
\boxed{\alpha_m^2=\frac{A}{3k\gamma(1+\beta X)}
=\frac{1}{3(1+\beta X)}\left[\frac{2M\mathrm{Ca}}{k(1+M)}-\beta\kappa_0\right]}.
$$

When $A\le0$, every nonzero mode decays, with a neutral zero-[wavenumber](../../../../../wavenumber.md) translation in the infinite-domain limit. For $\beta\kappa_0>0$, [surface-tension-gradient stabilization of viscous fingering](../../../../../surface-tension-gradient-stabilization-of-viscous-fingering.md) suppresses the instability entirely at positive injection speeds satisfying

$$
\boxed{0<U\le U_c=\frac{k\gamma\beta\kappa_0}{\mu_2-\mu_1},\qquad
\mathrm{Ca}\le\frac{k(1+M)\beta\kappa_0}{2M}}.
$$

If $\beta\kappa_0\le0$, no positive injection speed eliminates every long-wave unstable mode in an unbounded interface. The prescribed wetting variation is treated as an effective normal pressure law for [porous-media flow](../../../../../porous-media-flow-split.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
