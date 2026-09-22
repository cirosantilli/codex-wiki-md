<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use first-order [time-dependent perturbation theory](../../../../time-dependent-perturbation-theory.md), setting $c_1=1$ in the equation for $c_2$ and retaining the generally complex [matrix element](../../../../matrix-element.md) $d=\langle\psi_2|\widehat D_0|\psi_1\rangle$. With $\delta=\omega_0-\omega$ and $\Sigma=\omega_0+\omega$, the [probability amplitude](../../../../probability-amplitude.md) is

$$
c_2(t)=-\frac{id}{2\hbar}\int_{-\infty}^t e^{-b|s|}\{e^{i\delta s}+e^{i\Sigma s}\}\,ds.
$$

For $t>0$, split the [integral](../../../../integral-split.md) at the pulse maximum. For either $x=\delta$ or $x=\Sigma$,

$$
\begin{aligned}
F(x,t)&=\int_{-\infty}^0e^{(b+ix)s}ds+\int_0^te^{(-b+ix)s}ds\\
&=\frac1{b+ix}+\frac{1-e^{(-b+ix)t}}{b-ix}
=\frac{2b}{b^2+x^2}-\frac{e^{(-b+ix)t}}{b-ix}.
\end{aligned}
$$

Thus the full first-order answer, without discarding the counter-rotating contribution, is

$$
\boxed{c_2(t)=-\frac{id}{2\hbar}\{F(\delta,t)+F(\Sigma,t)\},\qquad t>0.}
$$

At long times it gives

$$
\boxed{P_2(\infty)=\frac{|d|^2b^2}{\hbar^2}
\left(\frac1{b^2+\delta^2}+\frac1{b^2+\Sigma^2}\right)^2.}
$$

This full expression is not exactly one squared [Lorentzian line shape](../../../../lorentzian-line-shape.md). To obtain the intended near-[resonance](../../../../resonance.md) [spectral line](../../../../spectral-line.md) profile, additionally assume $b,|\delta|\ll\omega_0$, so the pulse has a narrow positive-[frequency](../../../../frequency.md) lobe and $F(\Sigma,t)$ is negligible. Then

$$
c_2(t)\simeq-\frac{id}{2\hbar}\left[\frac{2b}{b^2+\delta^2}-\frac{e^{(-b+i\delta)t}}{b-i\delta}\right],
\qquad
\boxed{P_2(\infty)\simeq\frac{|d|^2}{\hbar^2b^2}\frac1{[1+(\delta/b)^2]^2}.}
$$

The weak-excitation condition near [resonance](../../../../resonance.md) is $|d|/(\hbar b)\ll1$. The squared [Lorentzian line shape](../../../../lorentzian-line-shape.md) occurs because the symmetric exponential pulse has a [Lorentzian line shape](../../../../lorentzian-line-shape.md) _amplitude_ [Fourier transform](../../../../fourier-transform-split.md), which is then squared to obtain [probability](../../../../probability.md).

At half the maximum, $[1+(\delta/b)^2]^2=2$, so

$$
\boxed{\Delta\omega_{\rm FWHM}=2b\sqrt{\sqrt2-1}\simeq1.2872b,
\qquad\Delta\nu_{\rm FWHM}=\frac b\pi\sqrt{\sqrt2-1}.}
$$

The [full width at half maximum](../../../../full-width-at-half-maximum.md) refers to varying the drive [frequency](../../../../frequency.md) through the positive-[frequency](../../../../frequency.md) [resonance](../../../../resonance.md). For a concrete failure of the unqualified squared-[Lorentzian line shape](../../../../lorentzian-line-shape.md) claim, set $b=\omega=\omega_0$ while keeping $|d|/(\hbar b)\ll1$. The full first-order resonant [probability](../../../../probability.md) is $36/25$ times the one-lobe prediction. Weak radiation alone therefore does not justify dropping the second [Fourier transform](../../../../fourier-transform-split.md) lobe.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
