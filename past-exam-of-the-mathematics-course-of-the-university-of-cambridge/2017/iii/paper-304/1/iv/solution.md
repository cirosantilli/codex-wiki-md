<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The frequency-independent measure factor cancels in the ratio:

$$
R_N=\frac{\omega_2}{\omega_1}\prod_{r=1}^N\frac{1+(\beta\omega_2/(2\pi r))^2}{1+(\beta\omega_1/(2\pi r))^2}.
$$

Upon [analytic continuation](../../../../../../analytic-continuation.md) in frequency, this has [poles](../../../../../../pole.md) at $\omega_1=0,\ \pm2\pi i r/\beta$ and zeros at $\omega_2=0,\ \pm2\pi i r/\beta$, for $1\leq r\leq N$, apart from cancellations when numerator and denominator vanish together. They match those of $\sinh(\beta\omega_2/2)/\sinh(\beta\omega_1/2)$. To justify equality, rather than merely matching this divisor, use the [hyperbolic-sine infinite product](../../../../../../hyperbolic-sine-infinite-product.md)

$$
\frac{\sinh(\beta\omega/2)}{\beta\omega/2}=\prod_{r=1}^\infty\left[1+\left(\frac{\beta\omega}{2\pi r}\right)^2\right].
$$

It follows from pairing the [Weierstrass product for the reciprocal gamma function](../../../../../../weierstrass-product-for-the-reciprocal-gamma-function.md) at opposite imaginary arguments and using the [Gamma reflection formula](../../../../../../gamma-reflection-formula.md). Normal convergence on compact sets follows from $\sum r^{-2}<\infty$. Thus, for positive real frequencies,

$$
\boxed{\lim_{N\to\infty}R_N=\frac{\sinh(\beta\omega_2/2)}{\sinh(\beta\omega_1/2)}=\frac{\mathcal Z(\omega_1,\beta)}{\mathcal Z(\omega_2,\beta)}.}
$$

The cutoff ratio determines the frequency dependence, agreeing with the [thermal partition function of a quantum harmonic oscillator](../../../../../../thermal-partition-function-of-a-quantum-harmonic-oscillator.md).

The printed assertion about an absolute $\lim_N\mathcal Z_N$ needs a normalization qualification: independence of $A_N$ from $\omega$ alone does not ensure existence of a nonzero limit. Set $B_N=A_N\prod_{r=1}^N\nu_r^{-2}$. Then $\mathcal Z_N=B_N\omega^{-1}\prod_r(1+\omega^2/\nu_r^2)^{-1}$, so if $B_N\to B\ne0$, its limit is $B\beta/[2\sinh(\beta\omega/2)]$. The choice $B_N=1/\beta$ gives the required limit. Conversely, $B_N=(1+(-1)^N/2)/\beta$ is a positive frequency-independent normalization with no absolute limit, though every ratio above still converges. Matching zeros and poles alone also permits nonvanishing [entire functions](../../../../../../entire-function.md); the convergent normalized product is what rules them out here.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
