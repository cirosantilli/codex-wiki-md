<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [stellar adiabatic exponents](../../../../../../stellar-adiabatic-exponent.md) are fixed-composition, constant-[specific entropy](../../../../../../specific-entropy.md) derivatives:

$$
\boxed{\Gamma_1=\left(\frac{\partial\log P}{\partial\log\rho}\right)_s,\qquad\frac{\Gamma_2-1}{\Gamma_2}=\left(\frac{\partial\log T}{\partial\log P}\right)_s,\qquad\Gamma_3-1=\left(\frac{\partial\log T}{\partial\log\rho}\right)_s.}
$$

The [chain rule](../../../../../../chain-rule.md) gives $\Gamma_1(\Gamma_2-1)/\Gamma_2=\Gamma_3-1$. Define the [pressure](../../../../../../pressure.md) derivatives $\chi_\rho=(\partial\log P/\partial\log\rho)_T$ and $\chi_T=(\partial\log P/\partial\log T)_\rho$. The [first law of thermodynamics](../../../../../../first-law-of-thermodynamics.md), with $du=Tds+P\,d\rho/\rho^2$, gives

$$
\Gamma_3-1=\frac{P\chi_T}{\rho T c_V},\qquad c_P-c_V=\frac{P}{\rho T}\frac{\chi_T^2}{\chi_\rho}.
$$

Combining this with $d\log P=\chi_\rho d\log\rho+\chi_Td\log T$ on an adiabat gives

$$
\boxed{\Gamma_1=\chi_\rho+\chi_T(\Gamma_3-1)=\chi_\rho\frac{c_P}{c_V},\qquad\gamma\equiv\frac{c_P}{c_V}=\frac{\Gamma_1}{\chi_\rho}.}
$$

Thus the [specific-heat ratio](../../../../../../heat-capacity-ratio.md) is not generally equal to the three [stellar adiabatic exponents](../../../../../../stellar-adiabatic-exponent.md).

For the mixture, $\chi_\rho=\beta$ and $\chi_T=4-3\beta$. The [specific heat capacity at constant volume](../../../../../../specific-heat-capacity-at-constant-volume.md), obtained by differentiating $u$ at fixed [mass density](../../../../../../density.md), is

$$
c_V=\mathcal R\frac{24-21\beta}{2\beta}.
$$

Therefore the [adiabatic exponents of a monatomic gas-radiation mixture](../../../../../../adiabatic-exponents-of-a-monatomic-gas-radiation-mixture.md) and its [specific-heat ratio](../../../../../../heat-capacity-ratio.md) are

$$
\boxed{\begin{aligned}
\Gamma_3-1&=\frac{8-6\beta}{24-21\beta},\\
\Gamma_1&=\frac{32-24\beta-3\beta^2}{24-21\beta},\\
\Gamma_2&=\frac{32-24\beta-3\beta^2}{24-18\beta-3\beta^2},\\
\gamma&=\frac{32-24\beta-3\beta^2}{\beta(24-21\beta)}=\frac{\Gamma_1}{\beta}.
\end{aligned}}
$$

If a relation involving only the exponents is wanted, eliminate $\beta$ from $\Gamma_1=\beta+(4-3\beta)(\Gamma_3-1)$:

$$
\gamma=\frac{\Gamma_1(4-3\Gamma_3)}{\Gamma_1-4\Gamma_3+4}\qquad(0<\beta\le1).
$$

For a pure monatomic [perfect gas](../../../../../../ideal-gas.md), $\beta=1$ and $\gamma=\Gamma_1=\Gamma_2=\Gamma_3=5/3$. For any calorically perfect gas with constant heat capacities, the same equality holds with its own $\gamma_g$. In a genuine gas-radiation mixture, $0<\beta<1$, $\gamma=\Gamma_1/\beta$ while the exponents are given separately above.

In the radiation limit, $\Gamma_1=\Gamma_2=\Gamma_3=4/3$ and the [adiabatic temperature gradient](../../../../../../adiabatic-temperature-gradient.md) is $1/4$. This follows independently from photon [entropy](../../../../../../entropy.md): a comoving volume $V$ has $S\propto VT^3$, so an adiabat obeys $T\propto V^{-1/3}$ and $P\propto V^{-4/3}$. However, **$c_P/c_V$ is singular in the pure-radiation limit**, not $4/3$. This is the [pure-radiation constant-pressure heat-capacity singularity](../../../../../../pure-radiation-constant-pressure-heat-capacity-singularity.md). The equation $P=aT^4/3$ fixes [temperature](../../../../../../temperature.md) whenever [pressure](../../../../../../pressure.md) is fixed, so an ordinary constant-pressure [temperature](../../../../../../temperature.md) derivative is not available; along the mixture limit $\gamma\to\infty$ and $\beta\gamma\to4/3$. For photons alone, mass-specific quantities additionally require a material mass label. The often quoted radiation index $4/3$ is its pressure-density adiabatic exponent, not a finite constant-pressure/constant-volume heat-capacity ratio.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
