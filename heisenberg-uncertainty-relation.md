# Heisenberg uncertainty relation

↑ **Parent:** [Robertson uncertainty principle](robertson-uncertainty-principle.md)

The [Heisenberg uncertainty relation](heisenberg-uncertainty-relation.md) constrains the [standard deviations](standard-deviation.md) of [position](position.md) and [momentum](momentum-split.md) in one preparation:

$$
\Delta x\,\Delta p\geq\frac{\hbar}{2}.
$$

On the real line, the [position operator](position-operator.md) $x$ acts by multiplication, and the [momentum operator](momentum-operator.md) is $p=-i\hbar\,d/dx$, with $\hbar$ the reduced [Planck constant](planck-constant.md). Their [canonical commutation relation](canonical-commutation-relation.md) $[x,p]=i\hbar I$ and the [Robertson uncertainty principle](robertson-uncertainty-principle.md) give the bound on normalized [quantum states](quantum-state.md) satisfying the moment and product-domain assumptions above; [Schwartz functions](schwartz-function.md) are a convenient sufficient class. Thus making a preparation more sharply localized in [position](position.md) forces a wider [momentum](momentum-split.md) distribution, even for ideal [measurement in quantum mechanics](quantum-measurement-split.md).

An explicit saturating example is the normalized [Gaussian wave packet](gaussian-wave-packet.md), for $\sigma>0$,

$$
\psi_\sigma(x)=(2\pi\sigma^2)^{-1/4}\exp\!\left(-\frac{x^2}{4\sigma^2}\right),\qquad |\psi_\sigma(x)|^2=\frac{1}{\sqrt{2\pi}\sigma}\exp\!\left(-\frac{x^2}{2\sigma^2}\right).
$$

The [wavefunction](wave-function-split.md) is a [probability amplitude](probability-amplitude.md); its squared magnitude is the [probability density function](probability-density-function.md), by the [Born rule](born-rule.md). That density is a [normal distribution](normal-distribution.md) of mean zero and [standard deviation](standard-deviation.md) $\Delta x=\sigma$, rather than a density whose width is read directly from the amplitude's exponent. With the unitary, negative-exponent convention for the [Fourier transform](fourier-transform-split.md), its [momentum](momentum-split.md) amplitude is

$$
\widetilde\psi_\sigma(p)=\frac{1}{\sqrt{2\pi\hbar}}\int_{-\infty}^{\infty}e^{-ipx/\hbar}\psi_\sigma(x)\,dx=\left(\frac{2\sigma^2}{\pi\hbar^2}\right)^{1/4}\exp\!\left(-\frac{\sigma^2p^2}{\hbar^2}\right).
$$

The [Gaussian integral](gaussian-integral.md) evaluates this [Fourier transform](fourier-transform-split.md). Consequently $|\widetilde\psi_\sigma(p)|^2$ is another [normal distribution](normal-distribution.md), with mean zero and [standard deviation](standard-deviation.md)

$$
\Delta p=\frac{\hbar}{2\sigma},\qquad \Delta x\,\Delta p=\frac{\hbar}{2}.
$$

For example, in dimensionless units with $\hbar=1$, $\sigma=1/2,1,2$ give $(\Delta x,\Delta p)=(1/2,1),(1,1/2),(2,1/4)$. The [Gaussian wave packets](gaussian-wave-packet.md) all saturate the same bound: narrowing one density broadens the other. More precisely, choose a reference length $L$ and set $X=x/L$, $P=pL/\hbar$; then $[X,P]=iI$, and the plotted widths are $\sigma/L$ and $L\Delta p/\hbar$.

<a id="image-position-and-momentum-probability-densities-for-three-minimum-uncertainty-gaussian-preparations-dimensionless-widths-0-5-1-and-2-in-position-give-reciprocal-momentum-widths-1-0-5-and-0-25"></a>
![](gaussian-position-momentum-uncertainty.png)

**[Figure 5](#image-position-and-momentum-probability-densities-for-three-minimum-uncertainty-gaussian-preparations-dimensionless-widths-0-5-1-and-2-in-position-give-reciprocal-momentum-widths-1-0-5-and-0-25). Position and momentum probability densities for three minimum-uncertainty Gaussian preparations: dimensionless widths 0.5, 1, and 2 in position give reciprocal momentum widths 1, 0.5, and 0.25**.

The [Heisenberg uncertainty relation](heisenberg-uncertainty-relation.md) connects localization to the cost in [kinetic energy](kinetic-energy.md). In a [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md) with [mass](mass.md) $m>0$ and [angular frequency](angular-frequency.md) $\omega>0$, the [variance](variance-split.md) contribution to the [expectation value](expectation-value.md) of the [energy](energy-split.md) is bounded using the [arithmetic-geometric mean inequality](arithmetic-geometric-mean-inequality.md):

$$
\frac{(\Delta p)^2}{2m}+\frac{m\omega^2(\Delta x)^2}{2}\geq\omega\Delta x\,\Delta p\geq\frac{\hbar\omega}{2}.
$$

The mean-dependent contributions are nonnegative. The [Gaussian eigenstate for a quadratic potential](gaussian-eigenstate-for-a-quadratic-potential.md) with $\sigma^2=\hbar/(2m\omega)$ and zero means reaches this [ground state](ground-state.md) energy. This is why the tradeoff is more than a limitation on preparation: it predicts an unavoidable positive minimum [energy](energy-split.md).

Heisenberg's original article appeared in March 1927 as "Über den anschaulichen Inhalt der quantentheoretischen Kinematik und Mechanik", Zeitschrift für Physik 43, pp. 172–198. Its abstract discusses simultaneous imprecision of canonically conjugate quantities and explanatory thought experiments. The precise [standard deviation](standard-deviation.md) formulation here distinguishes preparation spreads from a slogan about measurement disturbance. [W. Heisenberg, original 1927 article and publisher metadata](https://doi.org/10.1007/BF01397280).

**Table of contents**

- [Confinement energy bound from position support](confinement-energy-bound-from-position-support.md)
- [Preparation uncertainty](preparation-uncertainty.md)
- [Heisenberg's microscope](heisenberg-s-microscope.md)
- [Chirped Gaussian wave packet](chirped-gaussian-wave-packet.md)

## ↑ Ancestors (5)

1. [Robertson uncertainty principle](robertson-uncertainty-principle.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Chirped Gaussian wave packet](chirped-gaussian-wave-packet.md)
- [Confinement energy bound from position support](confinement-energy-bound-from-position-support.md)
- [Equality case of the Heisenberg uncertainty relation](equality-case-of-the-heisenberg-uncertainty-relation.md)
- [Gaussian variational energy for the harmonic oscillator](gaussian-variational-energy-for-the-harmonic-oscillator.md)
- [Harmonic-oscillator number-state second moments](harmonic-oscillator-number-state-second-moments.md)
- [Heisenberg's microscope](heisenberg-s-microscope.md)
- [Heisenberg uncertainty relation](heisenberg-uncertainty-relation.md)
- [Nobel Prize in Physics in 1932](nobel-prize-in-physics-in-1932.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2021/section-a/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/16b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-b/b9/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-a/1/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1/section-b/b7/c/solution.md)
- [Preparation uncertainty](preparation-uncertainty.md)
