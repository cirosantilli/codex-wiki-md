<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\xi=z-Vt$ increase into the liquid, with the planar [solidification](../../../../../freezing.md) front at $\xi=0$. Denote the common [thermal conductivity](../../../../../thermal-conductivity.md) by $K=\rho c_p\kappa$. A bounded travelling [temperature](../../../../../temperature.md) profile satisfies $\kappa T''+VT'=0$. In the solid, boundedness as $\xi\to-\infty$ forces $T_s=T_m$; in the liquid,

$$
T_l(\xi)=T_\infty+\Delta T\,e^{-V\xi/\kappa}.
$$

The [Stefan condition](../../../../../stefan-condition.md) then gives

$$
\rho LV=K(T_s'(0)-T_l'(0))
=\rho c_pV\Delta T,
\qquad
\boxed{S=\frac{L}{c_p\Delta T}=1}.
$$

Thus the [travelling solidification front in a pure supercooled melt](../../../../../travelling-solidification-front-in-a-pure-supercooled-melt.md) releases just enough [latent heat](../../../../../latent-heat.md) to warm the initially supercooled liquid to $T_m$. There is no separate imposed [heat flux](../../../../../heat-flux-density.md) at infinity in this bounded travelling-wave problem.

For the interface perturbation write $\xi=\zeta(y,t)=\widehat\zeta e^{i\alpha y+\sigma t}$. Use the [Gibbs--Thomson relation](../../../../../gibbs-thomson-relation.md) for [curvature-induced melting-temperature depression](../../../../../curvature-induced-melting-temperature-depression.md)

$$
T_I=T_m-\Gamma\mathcal K,\qquad
\Gamma=\frac{\gamma T_m}{\rho L}.
$$

Here $\gamma$ is the [solid-liquid surface energy](../../../../../solid-liquid-surface-energy.md), $T_m$ in this expression is absolute [temperature](../../../../../temperature.md) in kelvin, and $\mathcal K$ is the sum of [principal curvatures](../../../../../principal-curvature.md), positive for solid convex into liquid. For this graph, $\mathcal K=-\zeta_{yy}=\alpha^2\zeta$. If [mean curvature](../../../../../mean-curvature.md) is defined as half this sum, $\mathcal K=2H$; this fixes the capillary factor unambiguously.

Under the [small-wavelength thermal approximation for a solidification front](../../../../../small-wavelength-thermal-approximation-for-a-solidification-front.md), take harmonic perturbation [temperatures](../../../../../temperature.md) that decay away from the interface:

$$
\theta_s=A_s e^{\alpha\xi}e^{i\alpha y+\sigma t},\qquad
\theta_l=A_l e^{-\alpha\xi}e^{i\alpha y+\sigma t}.
$$

This approximates their [temperature](../../../../../temperature.md) equation by Laplace's equation, neglecting perturbation time dependence and the moving-frame advection. Expanding the interfacial [temperature](../../../../../temperature.md) at the displaced surface gives

$$
A_s=-\Gamma\alpha^2\widehat\zeta,\qquad
A_l=\left(\frac{V\Delta T}{\kappa}-\Gamma\alpha^2\right)\widehat\zeta.
$$

The second expression includes displacement through the negative base liquid gradient. Linearizing the [Stefan condition](../../../../../stefan-condition.md) also requires evaluation of the base gradient at the displaced surface:

$$
\rho L\sigma\widehat\zeta
=K\left(\alpha A_s+\alpha A_l
-\frac{V^2\Delta T}{\kappa^2}\widehat\zeta\right).
$$

Using $S=1$ gives the requested reduced [dispersion relation](../../../../../dispersion-relation.md):

$$
\boxed{\sigma=-\frac{V^2}{\kappa}+V\alpha
-\frac{2\kappa\Gamma}{\Delta T}\alpha^3},
$$

or

$$
\boxed{\frac{\kappa\sigma}{V^2}
=-1+\frac{\kappa\alpha}{V}
-\frac{2\gamma T_m}{\rho L\Delta T}
\frac{\kappa^2\alpha^3}{V^2}}.
$$

The destabilizing $V\alpha$ term describes a protrusion entering colder liquid. The cubic term expresses stabilization by the curvature-induced [temperature](../../../../../temperature.md) decrease.

There is an important accuracy qualification. The harmonic approximation gives the leading short-wave thermal exponents, but the retained constant term is not a uniformly controlled next-order correction to the full moving-boundary problem. If perturbation diffusion is retained, its exponents are

$$
r_s=Q-\frac{V}{2\kappa},\quad
r_l=-Q-\frac{V}{2\kappa},\quad
Q=\sqrt{\alpha^2+\frac{V^2}{4\kappa^2}+\frac{\sigma}{\kappa}}.
$$

Substitution into exactly the same linearized boundary balances gives the [full thermal stability of a travelling solidification front](../../../../../full-thermal-stability-of-a-travelling-solidification-front.md):

$$
\boxed{\sigma=
\left(V-\frac{2\kappa\Gamma\alpha^2}{\Delta T}\right)Q
-\frac{V^2}{2\kappa}}.
$$

For example, with capillarity removed, $\sigma=V\alpha$ solves this relation exactly, whereas the harmonic reduction gives $V\alpha-V^2/\kappa$. The difference is smaller than the leading term when $\alpha\gg V/\kappa$, but demonstrates why the reduced formula should not be asserted as an exact dispersion law or a precise onset calculation. To neglect perturbation time dependence one also needs $|\sigma|\ll\kappa\alpha^2$; extremely large capillary damping is outside that approximation.

To analyse the displayed cubic, define

$$
q=\frac{\kappa\alpha}{V},\qquad
R_c=\frac{\kappa}{V}\frac{\rho L\Delta T}{\gamma T_m}.
$$

Then $\kappa\sigma/V^2=g(q)=-1+q-2q^3/R_c$. It is negative at zero and at sufficiently large $q$. Its positive stationary point is the unique maximum:

$$
q_*=\sqrt{R_c/6},\qquad
g(q_*)=-1+\frac23\sqrt{R_c/6}.
$$

Thus the [capillary threshold of a reduced solidification dispersion](../../../../../capillary-threshold-of-a-reduced-solidification-dispersion.md) is

$$
\boxed{R_c>\frac{27}{2}},
$$

with equality giving a neutral maximum and strict inequality giving a band of unstable positive [wavenumbers](../../../../../wavenumber.md). At equality, however, $q_*=3/2$, not $q_*\gg1$. The number $27/2$ is therefore **the threshold of the stated reduced cubic**, not a controlled threshold of the full thermal problem under the stated short-wave ordering. Far above this threshold its fastest-growing scale does satisfy $q_*\gg1$, making the short-wave mechanism meaningful.

The analogy for a [snowflake](../../../../../snowflake.md) is [dendritic growth of a snowflake](../../../../../dendritic-growth-of-a-snowflake.md). A protrusion has better access to the driving supersaturation or undercooling and grows faster than a sheltered region; this amplifies tips and promotes branching into [crystal dendrites](../../../../../dendrite-crystal.md). Interfacial capillarity suppresses arbitrarily fine tips. In an actual [snowflake](../../../../../snowflake.md), the main growth is deposition from water vapour, so the diffusion field and its driving variable differ from this pure-melt thermal example. The [hexagonal ice crystal anisotropy](../../../../../hexagonal-ice-crystal-anisotropy.md) supplies six equivalent preferred arm directions; an isotropic planar stability calculation alone cannot predict six arms. Nonlinear tip selection, vapour transport and side branching are needed for the later detailed morphology. The analysis explains the competition between diffusion-driven protrusion growth and capillary smoothing, with this physically necessary qualification.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
