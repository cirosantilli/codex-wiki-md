<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $S$ denote specific entropy, reserving $s$ from the first question for envelope thickness. The [stellar adiabatic exponents](../../../../../stellar-adiabatic-exponent.md) are defined at fixed composition by

$$
\boxed{\Gamma_1=\left(\frac{\partial\log P}{\partial\log\rho}\right)_S,
\qquad \frac{\Gamma_2-1}{\Gamma_2}
=\left(\frac{\partial\log T}{\partial\log P}\right)_S.}
$$

It is useful to introduce $\Gamma_3-1=(\partial\log T/\partial\log\rho)_S$, so $(\Gamma_2-1)/\Gamma_2=(\Gamma_3-1)/\Gamma_1$.

Take the stellar gas to be a fully ionized, nonrelativistic monatomic [ideal gas](../../../../../ideal-gas.md), with fixed specific gas constant $\mathcal R$. Its mixture with thermal radiation has

$$
P=\mathcal R\rho T+\frac13a_{\rm r}T^4,\qquad
u=\frac32\mathcal RT+\frac{a_{\rm r}T^4}{\rho}.
$$

Here $u$ is specific internal energy, and the [stellar gas-pressure fraction](../../../../../stellar-gas-pressure-fraction.md) is $\beta=\mathcal R\rho T/P$. The assumption of monatomic gas fixes its heat capacity; the perfect-gas [pressure](../../../../../pressure.md) law alone would not determine it.

At fixed $T$ and fixed $\rho$, respectively, the [pressure](../../../../../pressure.md) derivatives are

$$
\chi_\rho=\left(\frac{\partial\log P}{\partial\log\rho}\right)_T=\beta,
\qquad
\chi_T=\left(\frac{\partial\log P}{\partial\log T}\right)_\rho=4-3\beta.
$$

For an [isentropic process](../../../../../isentropic-process.md), the [first law of thermodynamics](../../../../../first-law-of-thermodynamics.md) gives $du=P\,d\rho/\rho^2$. Differentiate the internal energy rather than artificially holding $\beta$ fixed during the perturbation:

$$
\left(\frac32\mathcal R+\frac{4a_{\rm r}T^3}{\rho}\right)dT
=\frac{P+a_{\rm r}T^4}{\rho^2}d\rho.
$$

The parenthesis is $(P/\rho T)[(3/2)\beta+12(1-\beta)]$, giving

$$
\Gamma_3-1=\frac{4-3\beta}{12-(21/2)\beta}
=\frac{8-6\beta}{24-21\beta}.
$$

Since $d\log P=\chi_\rho d\log\rho+\chi_Td\log T$,

$$
\boxed{\Gamma_1=\beta+(4-3\beta)(\Gamma_3-1)
=\frac{32-24\beta-3\beta^2}{24-21\beta}.}
$$

Using the relation between the exponents gives the [adiabatic exponents of a monatomic gas-radiation mixture](../../../../../adiabatic-exponents-of-a-monatomic-gas-radiation-mixture.md)

$$
\boxed{\Gamma_2=\frac{32-24\beta-3\beta^2}{24-18\beta-3\beta^2},\qquad
\nabla_{\rm ad}=\frac{\Gamma_2-1}{\Gamma_2}
=\frac{8-6\beta}{32-24\beta-3\beta^2}.}
$$

The requested values, including the [adiabatic temperature gradient](../../../../../adiabatic-temperature-gradient.md), are

$$
\boxed{\begin{array}{c|ccc}
\beta&\Gamma_1&\Gamma_2&\nabla_{\rm ad}\\\hline
0&4/3&4/3&1/4\\
1/2&77/54&77/57&20/77\\
1&5/3&5/3&2/5
\end{array}.}
$$

The pure-radiation and pure-gas rows are understood as limits of the mixture.

For uniform composition, the [Schwarzschild criterion](../../../../../schwarzschild-criterion.md) for [stellar convective instability](../../../../../stellar-convective-instability.md) is

$$
\boxed{\nabla\equiv\frac{d\log T}{d\log P}>\nabla_{\rm ad}
=\frac{\Gamma_2-1}{\Gamma_2}.}
$$

To test whether a radiative configuration becomes unstable, use its required [stellar radiative temperature gradient](../../../../../stellar-radiative-temperature-gradient.md) $\nabla_{\rm rad}$ for $\nabla$. Since $dP/dr<0$, the equivalent radial condition is

$$
-\frac{dT}{dr}>\frac{\Gamma_2-1}{\Gamma_2}\frac TP\left(-\frac{dP}{dr}\right).
$$

An outward-displaced parcel then cools less than its new surroundings, remains less dense at the same [pressure](../../../../../pressure.md), and is further accelerated outward.

The requested [Eddington-model convective-core mass fraction](../../../../../eddington-model-convective-core-mass-fraction.md) follows from the usual global constant-$\beta$ closure. At the outer radiative surface, put $m=M$, $L_r=L$, and $P_{\rm rad}=(1-\beta)P$. Dividing the radiation-pressure gradient by the [stellar hydrostatic equation](../../../../../hydrostatic-pressure-support-equation.md) gives

$$
\frac{dP_{\rm rad}}{dP}=\frac{\kappa L_r}{4\pi cGm},\qquad
L=\frac{4\pi cGM}{\kappa}(1-\beta)=(1-\beta)L_{\rm Edd}.
$$

There is no energy generation outside the [convective core](../../../../../convective-core.md), so use $L_r=L$ there. The local radiative-gradient formula is

$$
\nabla_{\rm rad}(m)=\frac{3\kappa L P}{16\pi a_{\rm r}cGmT^4}
=\frac{\kappa L}{16\pi cGm(1-\beta)}\simeq\frac{M}{4m}.
$$

The same representative $\beta$ has been used in the global [luminosity](../../../../../luminosity.md) closure and at the boundary. Setting this gradient equal to $\nabla_{\rm ad}$ at $m=M_c$ produces

$$
\boxed{\frac{M_c}{M}=\frac1{4\nabla_{\rm ad}}
=\frac{\Gamma_2}{4(\Gamma_2-1)}
=\frac{32-24\beta-3\beta^2}{4(8-6\beta)}.}
$$

This is $1$, $77/80$, and $5/8$ for $\beta=0,1/2,1$, respectively, with $\beta=0$ a marginal radiation-dominated limit.

There is a consistency qualification to this last model estimate. **It cannot be an exact stellar solution if all the printed assumptions are enforced pointwise.** An exactly uniform nonzero radiation fraction would give $dP_{\rm rad}/dP=1-\beta$ at every radiative point. The exact equations would then require

$$
\frac{L_r}{m}=\frac{4\pi cG}{\kappa}(1-\beta).
$$

If $L_r$ is constant throughout an envelope with positive [mass density](../../../../../density.md), $m$ increases with radius, so this equality cannot hold there. Equivalently uniform $\beta$ fixes the actual gradient to $1/4$, whereas $\nabla_{\rm ad}>1/4$ for $\beta>0$. The boxed core fraction is the intended Eddington closure and boundary estimate, which relaxes exact constancy of $\beta$ in the detailed envelope. The [constant-beta radiative-envelope obstruction](../../../../../uniform-gas-pressure-fraction-and-constant-luminosity-radiative-envelope-incompatibility.md) identifies the missing approximation; it is not legitimate to silently assert exact compatibility.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
