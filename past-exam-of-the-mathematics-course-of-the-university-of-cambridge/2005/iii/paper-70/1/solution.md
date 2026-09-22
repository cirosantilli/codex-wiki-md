<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Buoyancy and the convective criterion.** Consider a small fluid parcel displaced outward by $\delta r$. Assume that sound waves keep its [pressure](../../../../../pressure.md) equal to the ambient [pressure](../../../../../pressure.md), while heat exchange is slow enough that its displacement is an [adiabatic process](../../../../../adiabatic-process.md). Composition is uniform, so the parcel and its surroundings have the same [mean molecular weight](../../../../../mean-molecular-weight.md). For an [ideal gas](../../../../../ideal-gas.md), $P\propto\rho T$, and an adiabatic parcel obeys $P\propto\rho^\gamma$. If $\delta\ln P<0$ is the [pressure](../../../../../pressure.md) change on moving outward, then

$$
\delta\ln\rho_{\rm parcel}=\frac1\gamma\delta\ln P,\qquad
\delta\ln\rho_{\rm ambient}=(1-\nabla)\delta\ln P.
$$

The [density](../../../../../density.md) excess of the parcel at its new location is therefore

$$
\delta\ln\rho_{\rm parcel}-\delta\ln\rho_{\rm ambient}
=\left[\nabla-\frac{\gamma-1}{\gamma}\right]\delta\ln P.
$$

If $\nabla>(\gamma-1)/\gamma$, this excess is negative: the outward-displaced parcel is lighter and accelerates farther outward. A downward displacement similarly continues downward. Conversely, a smaller gradient gives a restoring buoyancy force. The [Schwarzschild criterion](../../../../../schwarzschild-criterion.md) is thus stability for $\nabla<\nabla_{\rm ad}$ and instability for $\nabla>\nabla_{\rm ad}$, where the [adiabatic temperature gradient](../../../../../adiabatic-temperature-gradient.md) is $\nabla_{\rm ad}=(\gamma-1)/\gamma$. For a monatomic gas,

$$
\boxed{\gamma=5/3\quad\Longrightarrow\quad\nabla_{\rm ad}=2/5.}
$$

A composition gradient would require the additional [density](../../../../../density.md) effect in the [Ledoux criterion](../../../../../ledoux-criterion.md); it is absent in this calculation.

**[Opacity](../../../../../opacity.md) and [pressure](../../../../../pressure.md).** The supplied [opacity](../../../../../opacity.md) is characteristic of a cool hydrogen-rich [stellar atmosphere](../../../../../stellar-atmosphere.md) dominated by [negative hydrogen ion opacity](../../../../../negative-hydrogen-ion-opacity.md). Mostly neutral hydrogen can attach electrons supplied by partially ionized metals; bound-free and free-free absorption involving the resulting $H^-$ ions produces a steep positive [temperature](../../../../../temperature.md) dependence. The weak [density](../../../../../density.md) dependence and strong [temperature](../../../../../temperature.md) sensitivity can be represented by local power-law fits. At fixed composition the given [pressure](../../../../../pressure.md) form is equivalent to $\kappa\propto\rho^{1/2}T^{17/2}$, because $P\propto\rho T$. This is an approximate fit over the relevant cool-atmosphere regime, not an exact [opacity](../../../../../opacity.md) law at all temperatures; molecular [opacity](../../../../../opacity.md) or hydrogen ionization eventually changes the regime.

For a geometrically thin atmosphere take the [surface gravity of a star](../../../../../surface-gravity-of-a-star.md) to be constant, $g_s=GM/R^2$. Combining $dP/dr=-\rho g_s$ with $d\tau/dr=-\kappa\rho$ gives [hydrostatic equilibrium in optical depth](../../../../../hydrostatic-equilibrium-in-optical-depth.md),

$$
\frac{dP}{d\tau}=\frac{g_s}{\kappa_0P^{1/2}T^8}.
$$

The [grey atmosphere](../../../../../grey-atmosphere.md) relation gives $T^8=T_e^8(3\tau+2)^2/16$. With negligible external [pressure](../../../../../pressure.md), $P(0)=0$, integration yields

$$
\begin{aligned}
P^{3/2}(\tau)&=\frac{24g_s}{\kappa_0T_e^8}\int_0^\tau\frac{du}{(3u+2)^2}\\
&=\frac{8GM}{\kappa_0R^2T_e^8}\left(\frac12-\frac1{3\tau+2}\right).
\end{aligned}
$$

An imposed nonzero external [pressure](../../../../../pressure.md) would add $P(0)^{3/2}$; the boundary assumption is what fixes the integration constant here.

The factor in parentheses is $3\tau/[2(3\tau+2)]$. Hence

$$
\frac{d\ln T}{d\tau}=\frac3{4(3\tau+2)},\qquad
\frac{d\ln P}{d\tau}=\frac4{3\tau(3\tau+2)},\qquad
\nabla_{\rm rad}=\frac{9\tau}{16}.
$$

The [grey-atmosphere convection onset with eighth-power temperature opacity](../../../../../grey-atmosphere-convection-onset-with-eighth-power-temperature-opacity.md) occurs when this reaches $2/5$, so

$$
\boxed{\tau_c=\frac{32}{45}.}
$$

The radiative continuation below this boundary would be unstable. Efficient [convection](../../../../../convection.md) instead keeps the deeper star approximately adiabatic.

**Matching to the convective interior.** Write $P=K\rho^{5/3}$. Eliminating [density](../../../../../density.md) using the [ideal gas law](../../../../../ideal-gas-law.md) gives

$$
T=\frac\mu{\mathcal R}K^{3/5}P^{2/5},\qquad
K\propto T^{5/3}P^{-2/3}
$$

at fixed composition. Since $\tau_c$ is a fixed number, the matching [temperature](../../../../../temperature.md) $T_b$ is proportional to $T_e$, while the matching [pressure](../../../../../pressure.md) satisfies $P_b^{3/2}\propto g_sT_e^{-8}$. Consequently

$$
K\propto T_e^{5/3}\left(g_s^{2/3}T_e^{-16/3}\right)^{-2/3}
=T_e^{47/9}g_s^{-4/9}.
$$

The [polytropic mass-radius relation](../../../../../polytropic-mass-radius-relation.md) for index $3/2$ gives $K\propto RM^{1/3}$. Raising the matching relation to the ninth power and using $g_s\propto M/R^2$ therefore gives

$$
T_e^{47}\propto K^9g_s^4\propto R^9M^3\frac{M^4}{R^8}=RM^7.
$$

Finally the [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md) $L=4\pi R^2\sigma_{\rm SB}T_e^4$ yields the [Hayashi relation with eighth-power temperature opacity](../../../../../hayashi-relation-with-eighth-power-temperature-opacity.md),

$$
\boxed{L\propto R^{98/47}M^{28/47}.}
$$

Composition and the [opacity](../../../../../opacity.md) normalization are fixed in this comparison. The [entropy](../../../../../entropy.md) coefficient $K$ is spatially constant in each convective model, but need not be the same for stars with different masses or radii.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
