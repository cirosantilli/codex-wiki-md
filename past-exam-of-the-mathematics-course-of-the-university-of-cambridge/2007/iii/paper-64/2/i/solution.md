<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\mathcal H=a'/a$ and $\theta_N=i\mathbf k\cdot\mathbf v_N$. Choose the [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md) rest frame of [cold dark matter](../../../../../../cold-dark-matter.md), so $\theta_C=0$. Its continuity equation then gives $h'=-2\delta_C'$. Substitution in the trace Einstein equation gives

$$
\boxed{\delta_C''+\mathcal H\delta_C'
-\frac32\mathcal H^2(\Omega_C\delta_C+2\Omega_R\delta_R)=0.}
$$

For [radiation in cosmology](../../../../../../radiation-in-cosmology.md) the continuity and Euler equations are $\delta_R'+4\theta_R/3+2h'/3=0$ and $\theta_R'=k^2\delta_R/4$. Differentiate the first, eliminate $\theta_R'$ and $h''$, and obtain

$$
\boxed{\delta_R''+\frac{k^2}3\delta_R-\frac43\delta_C''=0.}
$$

[radiation in cosmology](../../../../../../radiation-in-cosmology.md) [pressure](../../../../../../pressure.md) supplies the acoustic restoring term while its [energy density](../../../../../../energy-density.md) contributes twice as strongly to the trace gravitational source through $1+3w_R=2$.

Deep in [radiation domination](../../../../../../radiation-domination.md), $a\propto\tau$, $\mathcal H=1/\tau$, $\Omega_R\simeq1$ and $\Omega_C\simeq0$. At long wavelengths $k\tau\ll1$, the [adiabatic initial conditions](../../../../../../adiabatic-initial-conditions.md) require $\delta_C=3\delta_R/4$. The cold-matter equation reduces to

$$
\delta_C''+\frac1\tau\delta_C'-\frac4{\tau^2}\delta_C=0.
$$

A power $\tau^p$ gives $p^2-4=0$. The regular growing solution therefore has

$$
\boxed{\delta_C=A(\mathbf k)\tau^2,\qquad
\delta_R=\frac43A(\mathbf k)\tau^2,\qquad k\tau\ll1.}
$$

The other adiabatic solution diverges as $\tau^{-2}$ and is discarded for the regular primordial growing mode. The relation between the [density contrasts](../../../../../../density-contrast.md) fixes their relative entropy to zero, not their subsequent equality inside the acoustic horizon.

One can also solve the leading radiation-era equations explicitly, which proves that the same regular mode develops logarithmic cold-matter growth after horizon entry. Put $x=k\tau/\sqrt3$. The first equation gives $\delta_R=(x^2\delta_{C,xx}+x\delta_{C,x})/3$. Substituting in the second gives

$$
x^2\delta_{C,xxxx}+5x\delta_{C,xxx}+x^2\delta_{C,xx}+x\delta_{C,x}=0.
$$

Define

$$
F(x)=\int_0^x\frac{1-\cos t}{t}dt+
\frac{\sin x}{x}-\frac{1-\cos x}{x^2}-\frac12.
$$

Its useful derivative is $F'=1/x-2\sin x/x^2+2(1-\cos x)/x^3$. Direct differentiation verifies the fourth-order equation and gives the associated [radiation in cosmology](../../../../../../radiation-in-cosmology.md) solution:

$$
\delta_C=K(\mathbf k)F(x),\qquad
\delta_R=\frac K3\left[-2\cos x+\frac{4\sin x}x
-\frac{4(1-\cos x)}{x^2}\right].
$$

At zero, $F=x^2/8+O(x^4)$ and $\delta_R=Kx^2/6+O(x^4)$, so this is precisely the regular [adiabatic radiation-era cold-dark-matter transfer solution](../../../../../../adiabatic-radiation-era-cold-dark-matter-transfer-solution.md) with $K=24A/k^2$. The other indicial behaviors of the fourth-order equation are $1,x,x^{-2}$; they are either nonadiabatic at leading order or singular and do not add another regular growing adiabatic mode.

For $x\gg1$, the integral is $\gamma+\ln x-\operatorname{Ci}(x)$, where $\gamma$ is the [Euler's constant](../../../../../../euler-s-constant.md) and $\operatorname{Ci}$ the [cosine integral](../../../../../../cosine-integral.md). Its oscillatory tail cancels the explicit leading $\sin x/x$ term, giving

$$
\delta_C=K\left[\ln x+\gamma-\frac12+O(x^{-2})\right],\qquad
\delta_R=-\frac{2K}3\cos x+O(x^{-1}).
$$

Thus the requested late sound-horizon behavior is

$$
\boxed{\delta_C\simeq B(\mathbf k)\ln(\tau/\tau_*),\qquad
\delta_R\simeq C(\mathbf k)\cos(k\tau/\sqrt3)+D(\mathbf k)\sin(k\tau/\sqrt3).}
$$

An additive constant in $\delta_C$ is absorbed into the reference $\tau_*$; the regular adiabatic solution fixes the acoustic phase, with $D=0$ in the explicit time-origin convention above. A general acoustic mixture has both terms. The physical expansion parameter is $k\tau/\sqrt3$; comparisons with $2\pi/k$ describe the same long- and short-wavelength regimes up to fixed numerical factors.

The contrast grows much more slowly after entry during [radiation domination](../../../../../../radiation-domination.md): [radiation in cosmology](../../../../../../radiation-in-cosmology.md) undergoes pressure-supported acoustic oscillations and cold matter only the logarithmic [Mészáros effect](../../../../../../meszaros-effect.md). Modes entering well before [matter-radiation equality](../../../../../../matter-radiation-equality.md) consequently have suppressed late amplitudes relative to modes that stay outside the horizon until near equality. After [matter domination](../../../../../../matter-domination.md) begins, pressureless growing modes can grow as $a$. This scale-dependent history produces the turnover and small-scale suppression of the matter transfer function and affects the initial conditions for [large-scale structure of the universe](../../../../../../large-scale-structure-of-the-universe-split.md). The early subhorizon limit requires both $k\tau\gg1$ and $\tau\ll\tau_{\rm eq}$; it is not applicable to a mode that enters only in the [matter domination](../../../../../../matter-domination.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
