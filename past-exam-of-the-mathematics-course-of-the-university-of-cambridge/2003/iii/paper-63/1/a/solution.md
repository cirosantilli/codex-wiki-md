<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Efficient [convection](../../../../../../convection.md) keeps the interior at nearly uniform [specific entropy](../../../../../../specific-entropy.md). For the fully ionized [monatomic gas](../../../../../../monatomic-gas.md), the [heat capacity ratio](../../../../../../heat-capacity-ratio.md) is $5/3$, so the [adiabatic process](../../../../../../adiabatic-process.md) gives $P=K_\rho\rho^{5/3}$, with $K_\rho$ spatially constant. The [ideal gas](../../../../../../ideal-gas.md) relation $P=\mathcal R\rho T/\mu$ then implies

$$
\boxed{P=KT^{5/2}},\qquad K=\left(\frac{\mathcal R}{\mu}\right)^{5/2}K_\rho^{-3/2}.
$$

The constant is spatial, not temporal: loss of [specific entropy](../../../../../../specific-entropy.md) during contraction changes it. This is a [stellar polytrope](../../../../../../stellar-polytrope.md) with [polytropic index](../../../../../../polytropic-index.md) $n=3/2$. We neglect [radiation pressure](../../../../../../radiation-pressure.md) and take the thin [photosphere](../../../../../../photosphere.md) as an atmospheric matching layer rather than a significant fraction of the stellar mass.

For a fixed dimensionless profile of the [Lane-Emden equation](../../../../../../lane-emden-equation.md), the [stellar homology](../../../../../../stellar-homology.md) relations have the form

$$
\rho_c=C_\rho\frac{M}{R^3},\qquad P_c=C_P\frac{GM^2}{R^4},\qquad T_c=\frac{C_P}{C_\rho}\frac{\mu GM}{\mathcal R R},
$$

where $C_\rho,C_P$ are positive dimensionless structure constants. More explicitly, write $\rho(r)=\rho_cf(x)$ and $m(r)=Mh(x)$ with $x=r/R$ and fixed dimensionless profiles. Mass conservation gives $M=4\pi\rho_cR^3\int_0^1f(x)x^2\,dx$. Integrating the [hydrostatic pressure support equation](../../../../../../hydrostatic-pressure-support-equation.md), with negligible surface pressure on the interior scale, gives $P_c=(GM\rho_c/R)\int_0^1h(x)f(x)x^{-2}\,dx$. Both integrals are fixed positive numbers, proving the two central scalings. Substituting these relations into $K=P_c/T_c^{5/2}$ gives

$$
\boxed{K=K_0\mu^{-5/2}M^{-1/2}R^{-3/2}},\qquad K_0=C_\rho^{5/2}C_P^{-3/2}\mathcal R^{5/2}G^{-3/2}.
$$

Thus the same [polytropic index](../../../../../../polytropic-index.md) fixes $K_0$ throughout this homologous sequence, while the dimensional [stellar polytrope](../../../../../../stellar-polytrope.md) constant changes.

At the [photosphere](../../../../../../photosphere.md), whose [optical depth](../../../../../../optical-depth.md) is $2/3$, identify the temperature with the [effective temperature](../../../../../../effective-temperature.md) $T_e$. The [ideal gas](../../../../../../ideal-gas.md) relation and the interior adiabat give $\rho_{\rm ph}=\mu K T_e^{3/2}/\mathcal R$. With the prescribed [opacity](../../../../../../opacity.md) and [stellar surface boundary condition](../../../../../../stellar-surface-boundary-condition.md),

$$
\kappa P=\frac{\kappa_0\mu}{\mathcal R}K^2T_e^8=\frac{2GM}{3R^2}.
$$

Eliminating $K$ therefore proves

$$
\boxed{T_e^8=\frac{2G\mathcal R}{3\kappa_0K_0^2}\mu^4M^2R}.
$$

Using the [Stefan–Boltzmann law](../../../../../../stefan-boltzmann-law.md), with $\sigma=ac/4$, gives the [luminosity](../../../../../../luminosity.md)

$$
L=4\pi R^2\sigma T_e^4=\pi ac\left(\frac{2G\mathcal R}{3\kappa_0}\right)^{1/2}K_0^{-1}\mu^2MR^{5/2}.
$$

The [gravitational energy of a stellar polytrope](../../../../../../gravitational-energy-of-a-stellar-polytrope.md) is $\Omega=-6GM^2/(7R)$ for $n=3/2$. The [stellar virial theorem](../../../../../../stellar-virial-theorem.md) for a [monatomic gas](../../../../../../monatomic-gas.md) gives $2U+\Omega=0$, and hence the total energy is $E=U+\Omega=-3GM^2/(7R)$. With no appreciable [stellar nuclear fusion](../../../../../../stellar-nuclear-fusion.md) or [accretion](../../../../../../accretion.md), energy conservation gives

$$
L=-\frac{dE}{dt}=-\frac{3GM^2}{7R^2}\dot R.
$$

Combining the two expressions for $L$ yields

$$
\dot R=-\frac{7\pi ac}{3}\left(\frac{2\mathcal R}{3\kappa_0G}\right)^{1/2}K_0^{-1}\mu^2M^{-1}R^{9/2}.
$$

Multiplication by $-7R^{-9/2}/2$ and integration proves the [contraction law with density-linear fourth-power stellar opacity](../../../../../../contraction-law-with-density-linear-fourth-power-stellar-opacity.md):

$$
\boxed{R^{-7/2}-R_0^{-7/2}=\frac{49\pi ac}{6}\left(\frac{2\mathcal R}{3\kappa_0G}\right)^{1/2}K_0^{-1}\mu^2M^{-1}(t-t_0)}.
$$

When the accumulated contraction term dominates the initial-radius term, $R\propto\mu^{-4/7}M^{2/7}(t-t_0)^{-2/7}$. Substitution into the central [ideal gas](../../../../../../ideal-gas.md) relation gives

$$
\boxed{T_c\propto\mu^{11/7}M^{5/7}(t-t_0)^{2/7}},
$$

which has the stated $t^{2/7}$ behavior when the time origin is negligible. This late-time approximation still requires the assumed [fully convective star](../../../../../../fully-convective-star.md), fixed composition and [opacity](../../../../../../opacity.md) law to remain applicable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
