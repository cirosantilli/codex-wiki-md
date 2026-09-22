<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $t_*$ be the observation time and normalize $a(t_*)=1$ temporarily. In pure [radiation domination](../../../../../../radiation-domination.md), $a(t)=(t/t_*)^{1/2}$ and $H_*=1/(2t_*)$. With $p(t)=T_r(t)=T_*/a(t)$, the proper speed is $v=[1+(ma/T_*)^2]^{-1/2}$. Put $u=\sqrt{t/t_*}=a(t)$ in the preceding integral. Since $dt=2t_*u\,du$,

$$
d=2t_*\int_0^1\frac{du}{\sqrt{1+(mu/T_*)^2}}=\boxed{H_*^{-1}\frac{T_*}{m}\operatorname{arsinh}\!\left(\frac m{T_*}\right).}
$$

The small-$m/T_*$ limit is $H_*^{-1}$, the radiation-era [particle horizon](../../../../../../particle-horizon.md). For $m/T_*\gg1$, the ratio is approximately $(T_*/m)\log(2m/T_*)$, retaining the distance accumulated while the particle was faster.

There is a normalization qualification: in arbitrary fixed [comoving coordinates](../../../../../../comoving-coordinate.md) the distance is $\chi=H_*^{-1}\operatorname{arsinh}(y)/(a_*y)$, $y=m/T_*$. The expression just derived is also the physical distance $L_*=a_*\chi$ at observation. Thus it equals a comoving distance only when $a_*=1$ is used, as in the preceding part. To express it in today's convention $a_0=1$, multiply $L_*$ by $1+z_*$. This is the [accumulated free-streaming distance in a radiation-dominated universe](../../../../../../accumulated-free-streaming-distance-in-a-radiation-dominated-universe.md).

Write $\omega_M=\Omega_Mh^2$, where $h$ here is the dimensionless present [Hubble constant](../../../../../../hubble-constant.md). The supplied equality [redshift](../../../../../../redshift.md) gives $1+z_{\rm eq}\simeq2.5\times10^4\omega_M$, and $T_{\rm eq}=T_0(1+z_{\rm eq})$. For $m=30\,\mathrm{eV}$ the requested dimensionless ratio is

$$
\boxed{\frac{L_{\rm eq}}{H_{\rm eq}^{-1}}=\frac{\operatorname{arsinh}(y_{\rm eq})}{y_{\rm eq}},\qquad y_{\rm eq}=\frac{30\,\mathrm{eV}}{T_0(1+z_{\rm eq})}.}
$$

The Hubble rate in this formula is the radiation-era extrapolation used in deriving it. A unique numerical ratio cannot be chosen without $\omega_M$.

**The printed [CMB](../../../../../../cosmic-microwave-background.md) [temperature](../../../../../../temperature.md) contains a factor-of-ten error.** Its $2.35\,\mathrm{meV}$ means $2.35\times10^{-3}\,\mathrm{eV}$, whereas the [cosmic microwave background temperature in energy units](../../../../../../cosmic-microwave-background-temperature-in-energy-units.md) is about $2.35\times10^{-4}\,\mathrm{eV}=0.235\,\mathrm{meV}$, corresponding to $2.725\,\mathrm K$. The [temperature](../../../../../../temperature.md) is supported by [NASA's CMB measurements](https://asd.gsfc.nasa.gov/archive/arcade/cmb_temperature.html). Using the printed value gives $y_{\rm eq}\simeq0.5106/\omega_M$; using the corrected value gives $y_{\rm eq}\simeq5.106/\omega_M$. For the illustrative choice $\Omega_M=1,h=0.5$, so $\omega_M=0.25$, these give respectively $T_{\rm eq}\simeq14.7$ and $1.47\,\mathrm{eV}$, and distance-to-Hubble-radius ratios about $0.716$ and $0.182$. This benchmark is an assumption for the estimate, not an extra parameter supplied by the paper.

For the present-day comoving length, use $H_r(z_{\rm eq})=H_0\sqrt{\Omega_M}(1+z_{\rm eq})^{3/2}$, the radiation contribution extrapolated to equality. Restoring $c$ for the conversion and using $c/H_0\simeq2998h^{-1}\,\mathrm{Mpc}$ gives

$$
\chi_0\simeq\frac{c}{H_0\sqrt{\Omega_M}\sqrt{1+z_{\rm eq}}}\frac{\operatorname{arsinh}(y_{\rm eq})}{y_{\rm eq}}\simeq\boxed{\frac{18.96}{\omega_M}\frac{\operatorname{arsinh}(y_{\rm eq})}{y_{\rm eq}}\,\mathrm{Mpc}.}
$$

For the same benchmark, this is about $54\,\mathrm{Mpc}$ using the printed [temperature](../../../../../../temperature.md) and $14\,\mathrm{Mpc}$ using the corrected [temperature](../../../../../../temperature.md), in the prescribed representative-momentum radiation-era model.

At equality matter is no longer negligible, so these are transition-era estimates. The actual total $H_{\rm eq}$ is $\sqrt2H_r(z_{\rm eq})$; inserting it in the simple normalization would lower the length by $\sqrt2$, but would not constitute an exact [integration](../../../../../../integral.md) through equality. An exact matter-plus-radiation treatment instead replaces the radiation integral by

$$
\chi_0=\frac{c}{H_0\sqrt{\Omega_r}}\int_0^{a_{\rm eq}}\frac{da}{\sqrt{1+a/a_{\rm eq}}\sqrt{1+(ma/p_0)^2}},\qquad a_0=1,
$$

with $p_0=T_0$ in the assumed model. This makes the order-one equality correction explicit. Real [neutrino](../../../../../../neutrino.md) [physical momenta in an FRW universe](../../../../../../physical-momentum-in-an-frw-universe.md) are distributed and their [temperature](../../../../../../temperature.md) need not equal the [photon](../../../../../../photon.md) [temperature](../../../../../../temperature.md); the calculation above follows the specified $p=T_r$ idealization.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
