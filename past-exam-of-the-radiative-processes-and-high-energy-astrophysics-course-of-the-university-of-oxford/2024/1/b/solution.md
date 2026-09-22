<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the ultrarelativistic regime of [a](../a.md), retaining a constant mean fractional [energy](../../../../energy-split.md) gain and ignoring losses gives, after $N$ individual crossings,

$$
\boxed{E_N\simeq E_0\left(1+\frac{u}{2c}\right)^N
\simeq E_0\exp\!\left(\frac{Nu}{2c}\right).}
$$

After $n$ complete return cycles, $N=2n$ and $E_n\simeq E_0(1+u/c)^n$, to the same first-order accuracy. These products approximate the mean amplification; individual [electron](../../../../electron.md) crossing angles give a distribution around it.

The downstream [electron](../../../../electron.md) distribution is nearly [isotropic](../../../../isotropy.md). Its crossing [particle flux](../../../../particle-flux.md) per unit area is $n_{\rm a}c/4$, where $n_{\rm a}$ is the accelerated-particle [number density](../../../../number-density.md). The downstream flow permanently advects particles away at [particle flux](../../../../particle-flux.md) $n_{\rm a}u_2$. Their ratio estimates the escape probability after a downstream visit:

$$
P_{\rm esc}\simeq\frac{n_{\rm a}u_2}{n_{\rm a}c/4}
=\frac{4u_2}{c}=\frac uc,
\qquad \boxed{P_{\rm ret}\simeq1-\frac uc.}
$$

Upstream particles are swept back towards the [shock wave](../../../../shock-wave.md) in this idealized infinite-upstream model. Consequently this return probability applies once per **complete cycle**, not once per individual crossing or local scattering event.

Let $A\simeq1+u/c$ be the amplification per complete cycle and $P=P_{\rm ret}$. A steady injection of $\mathcal N_0$ particles leaves $\mathcal N_0P^n$ surviving to reach $E=E_0A^n$. Eliminating $n$ gives the cumulative [power law](../../../../power-law.md) and differential [energy](../../../../energy-split.md) distribution

$$
\mathcal N(>E)\propto E^{\ln P/\ln A},\qquad
\frac{d\mathcal N}{dE}\propto E^{-s},\qquad
s=1-\frac{\ln P}{\ln A}\simeq2.
$$

The escape distribution has the same differential exponent when $P$ is independent of [energy](../../../../energy-split.md). Thus the standard [Strong-shock Rankine-Hugoniot conditions](../../../../strong-shock-rankine-hugoniot-conditions.md) give

$$
\boxed{\mathcal N(>E)\propto E^{-1},\qquad d\mathcal N/dE\propto E^{-2}.}
$$

Equivalently the phase-space [one-particle distribution function](../../../../one-particle-distribution-function.md) is $f(p)\propto p^{-4}$ for ultrarelativistic particles. Equal logarithmic intervals then contain equal particle [energy](../../../../energy-split.md). A finite source age, upstream escape, and radiative losses eventually introduce cutoffs or breaks.

A particle exponent is not automatically the [radiation spectral index](../../../../radiation-spectral-index.md). For [optically thin](../../../../optically-thin-medium.md) uncooled [synchrotron radiation](../../../../synchrotron-radiation.md) from $d\mathcal N/dE\propto E^{-s}$, the characteristic [frequency](../../../../frequency.md) scales as $\nu\propto E^2$ and the emitted [power](../../../../power.md) as $E^2$. Hence $L_\nu\propto E^{-s}E^2/(d\nu/dE)\propto\nu^{-(s-1)/2}$. With the convention $L_\nu\propto\nu^{-\alpha}$, this gives $\boxed{\alpha\simeq1/2}$ and $\nu L_\nu\propto\nu^{1/2}$. Strong [synchrotron cooling](../../../../synchrotron-cooling.md) steepens a continuously injected particle distribution by one exponent, giving $\alpha\simeq1$ above its cooling break. A [photon](../../../../photon.md) number distribution $d\dot N_\gamma/d\varepsilon\propto\varepsilon^{-\Gamma}$ has $\Gamma=\alpha+1$, or $3/2$ in the uncooled case.

**Convention qualification.** If the printed $P=1-u/c$ is instead imposed independently at every individual crossing, its combination with $A_{\rm crossing}=1+u/(2c)$ gives $s\simeq3$ and uncooled $\alpha\simeq1$. For example $u/c=0.01$ gives $s=1-\ln(0.99)/\ln(1.005)\simeq3.015$, whereas the consistent cycle model gives $s\simeq2.010$. The standard $s=2$ estimate requires matching the probability and amplification to the same complete cycle.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the radiative processes and high energy astrophysics course of the University of Oxford](../../../split.md)
5. [Radiative processes and high energy astrophysics course of the University of Oxford](../../../../radiative-processes-and-high-energy-astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
