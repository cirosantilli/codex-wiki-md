<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [renormalization-group beta function](../../../../../beta-function-physics.md) is

$$
\boxed{\beta(\lambda)=\left.\mu\frac{d\lambda}{d\mu}\right|_{\text{bare parameters fixed}}.}
$$

At one-loop accuracy, integrating $d\lambda/d\log\mu=b\lambda^2$ gives

$$
\boxed{\frac1{\lambda(\mu)}=\frac1{\lambda(\mu_0)}-b\log\frac\mu{\mu_0}.}
$$

For a positive weak coupling and $b>0$, the coupling increases toward the ultraviolet and decreases toward the infrared. Extrapolation predicts a [Landau pole](../../../../../landau-pole.md) at $\mu=\mu_0\exp[1/(b\lambda(\mu_0))]$, where the weak-coupling approximation fails. For $b<0$, the positive coupling decreases toward zero as $\mu\to\infty$: this is [asymptotic freedom](../../../../../asymptotic-freedom.md). Toward the infrared it instead grows, so perturbation theory eventually fails. The zero coupling is a fixed point. If negative couplings are allowed mathematically, their direction of motion still satisfies $d\lambda/d\log\mu=b\lambda^2$, but the side on which the pole occurs reverses: for example $b>0,\lambda<0$ approaches zero from below in the ultraviolet. Negative quartic coupling does not give a stable scalar potential.

For the loop calculation use $d=4-\epsilon$, $\epsilon>0$, and the PDF's vertex normalization $-\lambda\phi^4/4!$. A [Feynman parameter](../../../../../feynman-parameter.md) combines the denominators. Shift the Euclidean [loop momentum](../../../../../loop-momentum.md) to $\ell=k+xp$, and put $M_x^2=m^2+x(1-x)p^2$. The regulated integral without the vertex prefactor is

$$
I(p)=\mu^\epsilon\int_0^1dx\int\frac{d^d\ell}{(2\pi)^d}\frac1{(\ell^2+M_x^2)^2}.
$$

Using [Schwinger parameterization](../../../../../schwinger-parameterization.md), $q^{-2}=\int_0^\infty t e^{-tq}\,dt$, and the momentum [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
I(p)=\frac{\mu^\epsilon}{(4\pi)^{d/2}}\Gamma\left(2-\frac d2\right)
\int_0^1dx\,(M_x^2)^{d/2-2}.
$$

For $d=4-\epsilon$, $\Gamma(\epsilon/2)=2/\epsilon+O(1)$, while the other factors have finite limits. Thus the [massive scalar bubble pole in four dimensions](../../../../../massive-scalar-bubble-pole-in-four-dimensions.md) is

$$
\boxed{I(p)_{\rm div}=\frac1{8\pi^2\epsilon},\qquad
\left(\frac{i\lambda^2}{2}I(p)\right)_{\rm div}
=\frac{i\lambda^2}{16\pi^2\epsilon}.}
$$

This pole is independent of external [momentum](../../../../../momentum.md) and mass and hence is canceled by a local quartic [counterterm](../../../../../counterterm.md). There are three channels, corresponding to the three pairings of four external momenta. Their poles add, and a counterterm vertex $-i\delta\lambda$ cancels the sum when

$$
\boxed{\delta\lambda=\frac{3\lambda^2}{16\pi^2\epsilon},\qquad
\mathcal L_{\rm ct}^{(4)}=-\mu^\epsilon\frac{\delta\lambda}{4!}\phi^4.}
$$

This is the total counterterm for the three four-point diagrams specified here. The [minimal subtraction scheme](../../../../../minimal-subtraction-scheme.md) removes their poles only. The one-loop tadpole is momentum independent and requires a mass counterterm, but does not produce one-loop [wave-function renormalization](../../../../../wave-function-renormalization.md); that is why it does not alter this one-loop coupling calculation.

The dimensionful [bare coupling](../../../../../bare-coupling.md) is therefore

$$
\lambda_B=\mu^\epsilon\left[\lambda+\frac{a\lambda^2}{\epsilon}+O(\lambda^3)\right],
\qquad a=\frac3{16\pi^2}.
$$

Its independence of $\mu$ gives

$$
0=\epsilon\left(\lambda+\frac{a\lambda^2}{\epsilon}\right)
+\beta_d\left(1+\frac{2a\lambda}{\epsilon}\right)+O(\lambda^3).
$$

Putting $\beta_d=-\epsilon\lambda+b\lambda^2+O(\lambda^3)$, the finite coefficient of $\lambda^2$ is $b-a$. Thus

$$
\boxed{\beta_d=-\epsilon\lambda+\frac{3\lambda^2}{16\pi^2}+O(\lambda^3),\qquad
\beta_{d=4}=\frac{3\lambda^2}{16\pi^2}+O(\lambda^3).}
$$

This is the [one-loop quartic scalar beta function](../../../../../one-loop-quartic-scalar-beta-function.md), positive for nonzero weak real coupling. The factors would look different with a regulator $d=4-2\epsilon$, but the four-dimensional beta function is unchanged. For massless theory take nonexceptional external momentum, or an infrared regulator, so an infrared singularity is not confused with the ultraviolet pole.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
