<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The ultraviolet cutoff specifies which fluctuations remain explicit. Changing it integrates out some modes; to preserve long-distance predictions, their effect must be absorbed into the mass, interactions, and other couplings. Thus bare coefficients depend on $\Lambda$. The long-distance inverse [connected correlation function](../../../../../connected-correlation-function.md) has the form $\widetilde\Gamma(p)\simeq Z^{-1}(p^2+\xi^{-2})$. After fixing the gradient normalization, the infrared mass is an inverse [correlation length](../../../../../correlation-length.md). With the question's unrescaled gradient coefficient, $\xi^{-2}=\alpha m^2$ at Gaussian level, so proportionality rather than literal equality is appropriate until that normalization is chosen.

As a concrete [momentum-shell renormalization group](../../../../../momentum-shell-renormalization-group.md) step, split $\phi=\phi_<+\phi_>$ into modes below $\Lambda/b$ and in the shell $\Lambda/b<|p|<\Lambda$, and define

$$
e^{-H_{\rm eff}[\phi_<]}=\int\mathcal D\phi_>\,e^{-H[\phi_<+\phi_>]}.
$$

Then rescale coordinates and the field to restore the cutoff and gradient coefficient. A [local derivative expansion](../../../../../local-derivative-expansion.md) of $H_{\rm eff}$ gives new quadratic, quartic, and higher even couplings. If the system has short-range interactions, the field varies slowly, the effective potential is analytic, and remaining fluctuations are small, retaining the leading gradient and lowest stabilizing powers and minimizing the resulting functional gives [Landau-Ginzburg theory](../../../../../landau-ginzburg-theory.md). Suppressing the omitted fluctuations is the substantive [Landau approximation](../../../../../landau-approximation.md); it is justified sufficiently far from the narrow fluctuation region or above the appropriate [upper critical dimension](../../../../../upper-critical-dimension.md).

The truncated two-point function in this question is the [one-particle-irreducible two-point vertex](../../../../../one-particle-irreducible-two-point-vertex.md), $\widetilde\Gamma(p)=\widetilde G(p)^{-1}$. It is the Hessian of the Legendre effective action, not merely the connected two-point function. In perturbation theory,

$$
\widetilde\Gamma(p)=\widetilde G_0(p)^{-1}+\delta m^2+\Sigma(p).
$$

Here $\widetilde G_0$ is the Gaussian propagator about the chosen reference mass, $\delta m^2$ is the mass [counterterm](../../../../../counterterm.md) or bare-to-reference mass shift, and $\Sigma$ is the interaction [self-energy](../../../../../self-energy.md), computed from proper diagrams. Fix the gradient normalization so $\widetilde G_0(p)=(p^2+M^2)^{-1}$, and choose the infrared reference mass $M^2=m^2(0,T)$. Then $\delta m^2=m^2(\Lambda,T)-M^2$ at this order. The mass renormalization condition is $\widetilde\Gamma(0)=M^2$.

At one loop the only two-point diagram is the quartic [tadpole diagram](../../../../../tadpole-diagram.md). There are $4\cdot3$ choices for attaching its two external lines, leaving the other pair contracted; dividing by $4!$ gives its factor $1/2$. It is independent of external momentum, so

$$
\Sigma^{(1)}(p)=\frac g2\int_{|q|<\Lambda}\frac{d^Dq}{(2\pi)^D}\frac1{q^2+M^2}.
$$

The renormalization condition therefore gives the self-consistent one-loop equation

$$
\boxed{M^2=m^2(\Lambda,T)+\frac g2\int_{|q|<\Lambda}\frac{d^Dq}{(2\pi)^D}\frac1{q^2+M^2}.}
$$

Using $M$ inside the loop is a self-consistent resummation; replacing it by the bare mass gives the same formal first-order expansion away from infrared problems.

Subtract the equation at $T_c$, where $M=0$, and absorb regular temperature dependence of $g$ into the thermal coefficient. Let $\tau=m^2(\Lambda,T)-m^2(\Lambda,T_c)\propto T-T_c$ and $I(M)=\int_{|q|<\Lambda}d^Dq/(2\pi)^D(q^2+M^2)^{-1}$. Then

$$
\tau=M^2+\frac g2[I(0)-I(M)],\qquad I(0)-I(M)=\int_{|q|<\Lambda}\frac{d^Dq}{(2\pi)^D}\frac{M^2}{q^2(q^2+M^2)}.
$$

For $D>4$, the integral divided by $M^2$ tends to a finite cutoff-dependent constant, since its small-momentum radial integrand is $q^{D-5}$. Thus $\tau$ is proportional to $M^2$, consistent with the Landau prediction. For $2<D<4$, set $q=Mz$: the correction instead scales as $M^{D-2}$ and dominates $M^2$. At $D=4$ it is proportional to $M^2\log(\Lambda/M)$. Hence a pure linear Landau mass law without logarithmic modification is consistent only above

$$
\boxed{D_c=4.}
$$

For $D\leq2$, the massless integral itself is infrared divergent, so the subtraction already needs additional care. The sub-four-dimensional self-consistent approximation locates the breakdown of mean-field behavior; it is not an exact calculation of interacting critical exponents.

At a [tricritical point](../../../../../tricritical-point.md) the quartic coupling is tuned away and the leading stabilizing interaction is $g_6\phi^6$. At the [Gaussian fixed point](../../../../../gaussian-fixed-point.md), the field has [engineering dimension](../../../../../engineering-dimension.md) $(D-2)/2$, so the sextic coefficient rescales as $g_6'=b^{D-3(D-2)}g_6=b^{6-2D}g_6$. It changes from irrelevant to relevant at

$$
\boxed{D_c^{\rm tricritical}=3.}
$$

This is the sextic case of the [upper critical dimension of an even scalar interaction](../../../../../upper-critical-dimension-of-an-even-scalar-interaction.md); marginality at three dimensions allows logarithmic corrections.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
