<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take transverse length units in which the [wave phase](../../../../../../phase-waves.md) modulation has [wavenumber](../../../../../../wavenumber.md) one. Set $E_0(z)=e^{i\cos z}$. A [Taylor expansion](../../../../../../taylor-expansion.md) of the free parabolic propagator gives

$$
E(x,z)=E_0+\frac{ix}{2k}E_0''-\frac{x^2}{8k^2}E_0''''+O(x^3).
$$

For a general real [wave phase](../../../../../../phase-waves.md) $\phi$,

$$
\frac{E_0''}{E_0}=i\phi''-(\phi')^2,\qquad
\frac{E_0''''}{E_0}=i\phi''''-4\phi'\phi'''-3(\phi'')^2-6i(\phi')^2\phi''+(\phi')^4.
$$

Multiplying the envelope expansion by its [complex conjugate](../../../../../../complex-conjugate.md) and collecting powers of $x$ gives the [phase-to-intensity conversion near a deterministic phase screen](../../../../../../phase-to-intensity-conversion-near-a-deterministic-phase-screen.md),

$$
I=1-\frac{x}{k}\phi''+\frac{x^2}{k^2}\left[(\phi'')^2+\phi'\phi'''\right]+O(x^3).
$$

For $\phi=\cos z$, $\phi'=-\sin z$, $\phi''=-\cos z$ and $\phi'''=\sin z$, hence

$$
\boxed{I(x,z)=1+\frac{x}{k}\cos z+\frac{x^2}{k^2}\cos2z+O(x^3)}.
$$

The first-order brightening occurs where the [wave phase](../../../../../../phase-waves.md) curvature is negative. Both correction terms average to zero over a transverse period, in agreement with power conservation. If a dimensional modulation $\cos(qz)$ is used instead, the two terms are $(q^2x/k)\cos(qz)$ and $(q^4x^2/k^2)\cos(2qz)$.

<a id="3/c/image-phase-curvature-converts-a-unit-amplitude-sinusoidal-phase-screen-into-intensity-variations-exact-paraxial-propagation-is-compared-with-its-quadratic-near-screen-approximation"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80-phase-screen.png)

**[Figure 1](#3/c/image-phase-curvature-converts-a-unit-amplitude-sinusoidal-phase-screen-into-intensity-variations-exact-paraxial-propagation-is-compared-with-its-quadratic-near-screen-approximation). Phase curvature converts a unit-amplitude sinusoidal phase screen into intensity variations; exact paraxial propagation is compared with its quadratic near-screen approximation**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
