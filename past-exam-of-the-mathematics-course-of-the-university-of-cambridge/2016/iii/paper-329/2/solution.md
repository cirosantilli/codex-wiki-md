<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In the [surfactant transport with exchange relaxation](../../../../../surfactant-transport-with-exchange-relaxation.md), $DC/Dt$ is the [material derivative](../../../../../material-derivative.md) following an interfacial material element. The term $-C\nabla_s\cdot\mathbf u_s$ accounts for dilution by tangential stretching, while $-C(\mathbf u\cdot\mathbf n)\nabla_s\cdot\mathbf n$ accounts for changing area through normal motion and [curvature](../../../../../curvature.md). The [surface diffusion](../../../../../surface-diffusion.md) term redistributes [surfactant](../../../../../surfactant.md) down concentration gradients. The exchange term relaxes its concentration towards $C_0$, through adsorption or desorption from a surrounding reservoir, on time scale $k^{-1}$.

In the bubble frame the spherical interface is stationary and impermeable. A steady [material derivative](../../../../../material-derivative.md) is $\mathbf u_s\cdot\nabla_s C'$. For a linear response in the rising speed this and $C'\nabla_s\cdot\mathbf u_s$ are second order, whereas stretching of $C_0$ is first order. Thus

$$
\boxed{(D_s\Delta_s-k)C'=C_0\nabla_s\cdot\mathbf u_s.}
$$

Rotational symmetry, linear response to $\mathbf U$, and zero normal velocity allow only $\mathbf u_s=A P\mathbf U$, where $P=I-\mathbf n\mathbf n$ is the [surface tangent projector](../../../../../surface-tangent-projector.md). This is the dipolar, axisymmetric sector; axisymmetry alone, without the linear-response assumption, would allow other angular dependence.

On a sphere $\mathbf n=\mathbf x/r$ and $\partial_j n_i=(\delta_{ij}-n_i n_j)/r$. Applying the [surface tangent projector](../../../../../surface-tangent-projector.md) to the derivative gives the [sphere surface derivative identities](../../../../../sphere-surface-derivative-identities.md)

$$
\boxed{\nabla_s\mathbf n=P/a,\quad\nabla_s\cdot\mathbf n=2/a,\quad\Delta_s\mathbf n=-2\mathbf n/a^2,\quad\nabla_s\cdot(P\mathbf U)=-2(\mathbf U\cdot\mathbf n)/a.}
$$

For example, taking a second [surface divergence](../../../../../surface-divergence.md) of the first identity yields the third. Equivalently, the components of $\mathbf n$ are degree-one [spherical harmonics](../../../../../spherical-harmonic.md). Hence a [dipolar surfactant distribution](../../../../../dipolar-surfactant-distribution.md) solves the linear equation:

$$
\boxed{C'=B\mathbf U\cdot\mathbf n,\qquad B=\frac{2A C_0 a}{ka^2+2D_s}.}
$$

The required smallness condition is **$2|A|Ua/(ka^2+2D_s)\ll1$**. [Surface diffusion](../../../../../surface-diffusion.md) or exchange must smooth the concentration faster than it is redistributed by the actual interfacial velocity. We require $k\geq0$, $D_s\geq0$ and $ka^2+2D_s>0$; with neither process there is no such steady linear balance at nonzero $A$. A small [capillary number](../../../../../capillary-number.md) $\mu U/\gamma_0$ also justifies the spherical approximation.

Take the normal from the inner bubble to the outer liquid, define $[\sigma]_-^+=\sigma_+-\sigma_-$, and set $\kappa=\nabla_s\cdot\mathbf n$. The [interfacial stress balance with variable surface tension](../../../../../interfacial-stress-balance-with-variable-surface-tension.md) is

$$
\boxed{[\boldsymbol\sigma]_-^+\mathbf n=\gamma\kappa\mathbf n-\nabla_s\gamma.}
$$

Because $\nabla_s C'=B P\mathbf U/a$ and $\gamma=\gamma_0-\gamma_1C'$, its tangential part becomes

$$
\boxed{P[\boldsymbol\sigma]_-^+\mathbf n=\frac{6\mu A\lambda}{a}P\mathbf U,\qquad\lambda=\frac{\gamma_1 C_0 a}{3\mu(ka^2+2D_s)}.}
$$

This is a [Marangoni stress](../../../../../marangoni-effect.md): surface-tension gradients oppose the clean-bubble circulation.

Use the [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md), $\mathbf u=\nabla(\mathbf x\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi$ and $p=2\mu\nabla\cdot\boldsymbol\Phi$. The constant vector potential gives $\mathbf u\to-\mathbf U$. In the decaying, linear axisymmetric sector, a vector monopole and scalar dipole provide the two constants needed at the sphere; other equivalent potential choices amount to a representation freedom. The PDF potential contains the factor $a$ omitted in the TeX aid. With that factor restored, the exterior velocity is

$$
\mathbf u=-\mathbf U-\alpha a\left(\frac{\mathbf U}{r}+\frac{(\mathbf U\cdot\mathbf x)\mathbf x}{r^3}\right)+\beta a^3\left(-\frac{\mathbf U}{r^3}+\frac{3(\mathbf U\cdot\mathbf x)\mathbf x}{r^5}\right),\qquad p=-\frac{2\mu\alpha a\,\mathbf U\cdot\mathbf x}{r^3}.
$$

At the interface, no penetration gives $\beta-\alpha=1/2$, and the tangential velocity gives $A=-(1+\alpha+\beta)$. **Using the traction coefficient printed in equation (3)**, the tangential stress condition gives $2\beta=A\lambda$. The requested algebraic answers are therefore

$$
\boxed{A_{\rm printed}=-\frac1{2(1+\lambda)},\quad\alpha_{\rm printed}=-\frac{2+3\lambda}{4(1+\lambda)},\quad\beta_{\rm printed}=-\frac{\lambda}{4(1+\lambda)}.}
$$

**There is a factor-of-two error in the PDF traction.** Direct differentiation of the preceding velocity with the [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md) gives

$$
\boldsymbol\sigma\mathbf n=\frac{6\mu}{a}\left[\beta\mathbf U+(\alpha-3\beta)(\mathbf U\cdot\mathbf n)\mathbf n\right],
$$

rather than its printed coefficient $12\mu/a$. In particular the tangential [traction](../../../../../traction.md) is $6\mu\beta P\mathbf U/a$. Keeping the same definition of $\lambda$, the physically consistent [translating surfactant-coated bubble](../../../../../translating-surfactant-coated-bubble.md) instead has $\beta=A\lambda$ and

$$
\boxed{A=-\frac1{2(1+2\lambda)},\quad\alpha=-\frac{1+3\lambda}{2(1+2\lambda)},\quad\beta=-\frac{\lambda}{2(1+2\lambda)}.}
$$

The two sets must not be silently conflated. As a useful check, the no-slip limit has the usual total [Stokes flow](../../../../../stokes-flow-split.md) drag $6\pi\mu aU$ with the corrected [traction](../../../../../traction.md); the printed [traction](../../../../../traction.md) would double it.

Both versions give $A=-1/2$, $\alpha=-1/2$, $\beta=0$ when $\lambda\to0$: the interface is tangentially stress-free and circulates as a clean inviscid bubble. For $\lambda\to\infty$, $A\to0$, $\alpha\to-3/4$, $\beta\to-1/4$: the interface is immobile in the bubble frame and behaves as a no-slip sphere. The [Marangoni stress](../../../../../marangoni-effect.md) remains finite because $\lambda A$ has a nonzero limit. The concentration smallness condition still has to hold; large $\lambda$ is not by itself a complete linearization criterion.

The normal component is balanced by the inner gas pressure and the normal capillary stress $\gamma\kappa$, including the variation of $\gamma$, together with the [hydrostatic pressure](../../../../../hydrostatic-pressure.md) difference responsible for buoyancy. A spatially uniform inner pressure alone cannot balance the dipolar [traction](../../../../../traction.md). To make the [normal stress balance on a translating bubble](../../../../../normal-stress-balance-on-a-translating-bubble.md) explicit, let $\Delta\rho_b$ be the outer-minus-inner [mass density](../../../../../density.md). After removing the equilibrium Laplace pressure, the corrected outer normal [traction](../../../../../traction.md) has dynamic part $-3\mu(1+\lambda)(\mathbf U\cdot\mathbf n)/[a(1+2\lambda)]$. Its degree-one balance is

$$
\Delta\rho_bga\cos\vartheta-\frac{3\mu(1+\lambda)}{a(1+2\lambda)}U\cos\vartheta=-\frac{2\gamma_1 B}{a}U\cos\vartheta.
$$

Thus, if a terminal speed is desired, **$U=\Delta\rho_bga^2(1+2\lambda)/[3\mu(1+3\lambda)]$**, interpolating between the clean-bubble and rigid-sphere speeds. A degree-one shape displacement is merely a translation of the sphere, so the balance determines its rise speed, rather than a dipolar shape distortion.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 329](../../paper-329-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
