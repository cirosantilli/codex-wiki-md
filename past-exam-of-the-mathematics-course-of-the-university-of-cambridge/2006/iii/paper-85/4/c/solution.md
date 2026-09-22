<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The linearized complex equation couples a [perturbation](../../../../../../perturbation.md) and its conjugate, so a single complex [Fourier mode](../../../../../../fourier-mode.md) by itself is not a closed [perturbation](../../../../../../perturbation.md) ansatz. Equivalently use real [amplitude](../../../../../../wave-amplitude.md) and [wave phase](../../../../../../phase-waves.md) [perturbations](../../../../../../perturbation.md), with [Fourier modes](../../../../../../fourier-mode.md) paired to make each real field. Writing $A=A_0+\alpha+i\beta$ and $B=A_0^2$ gives

$$
\alpha_T=4\alpha_{XX}+(\mu+9\hat sB-50B^2)\alpha,\qquad
\beta_T=4\beta_{XX}+(\mu+3\hat sB-10B^2)\beta.
$$

A real [amplitude](../../../../../../wave-amplitude.md) mode of slow [wavenumber](../../../../../../wavenumber.md) $\ell>0$ therefore becomes neutral when

$$
\boxed{\mu-4\ell^2+9\hat sA_0^2-50A_0^4=0.}
$$

For a nonzero uniform state the [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) condition eliminates $\mu$, leaving [amplitude](../../../../../../wave-amplitude.md) growth $6\hat sB-40B^2-4\ell^2$. The [wave phase](../../../../../../phase-waves.md) mode growth is simply $-4\ell^2$, so it cannot give a nonzero-wavenumber bifurcation from these undetuned states.

The concave quadratic has maximum

$$
\max_{B\ge0}(6\hat sB-40B^2)=\frac{9\hat s^2}{40},\qquad B=\frac{3\hat s}{40}.
$$

Thus a nonzero uniform state needs $\ell\le3\hat s/(4\sqrt{10})$ to have a modulation bifurcation. The slow domain length is $\varepsilon^2L$, so $\ell_n=2\pi n/(\varepsilon^2L)$. If its smallest positive [wavenumber](../../../../../../wavenumber.md) already exceeds this bound, none can become neutral. Since $s=\varepsilon^2\hat s$, the conclusion is

$$
\boxed{L<\frac{8\pi\sqrt{10}}{3s}\ \Longrightarrow\
\text{no modulation bifurcation of a nonzero uniform state}.}
$$

This is the [modulation cutoff of a cubic-quintic uniform pattern](../../../../../../modulation-cutoff-of-a-cubic-quintic-uniform-pattern.md). If the bound is reversed, candidate squared amplitudes are $B=(3\hat s\pm\sqrt{9\hat s^2-160\ell^2})/40$. They lie on the lower branch; the upper branch is already damped in [amplitude](../../../../../../wave-amplitude.md) and cannot undergo this stationary modulation bifurcation.

The word “nonzero” is necessary in the final claim. At $A_0=0$, the [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) exists independently of $\mu$, and the mode growth is $\mu-4\ell^2$. It becomes neutral at $\mu=4\ell_n^2$ for every finite domain. For example, take $\hat s=1$, $\varepsilon^2L=20$: then $L=20/\varepsilon^2<8\pi\sqrt{10}/(3s)$, but the zero state has a first-sideband threshold at $\mu=\pi^2/25$. Therefore the printed assertion, if read to include the trivial state, is false. The derived domain-size bound is the correct statement for nonzero pattern branches.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
