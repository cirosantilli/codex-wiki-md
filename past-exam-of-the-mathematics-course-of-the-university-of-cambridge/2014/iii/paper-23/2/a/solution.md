<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [Poisson summation formula](../../../../../../poisson-summation-formula.md) to $h(x)=e^{2\pi i\tau x^2}$, with Fourier kernel $e^{-2\pi i x\xi}$. Its [complex Gaussian Fourier transform](../../../../../../complex-gaussian-fourier-transform.md) is

$$
\widehat h(\xi)=(-2i\tau)^{-1/2}e^{-\pi i\xi^2/(2\tau)}.
$$

Choose the square root holomorphic on the half-plane and positive when $\tau$ is positive imaginary. Summing over integer $\xi$ gives

$$
\boxed{\theta\left(-\frac1{4\tau}\right)=\sqrt{\frac{2\tau}{i}}\,\theta(\tau).}
$$

Here the printed [theta series of integer squares](../../../../../../theta-series-of-integer-squares.md) uses $q=e^{2\pi i\tau}$; the common theta-constant convention instead uses $e^{\pi iz}$.

To keep track of the shifted series, put $z=2\tau$ and define

$$
\Theta_3(z)=\sum_ne^{\pi izn^2},\quad\Theta_4(z)=\sum_n(-1)^ne^{\pi izn^2},\quad\Theta_2(z)=\sum_ne^{\pi iz(n+1/2)^2}.
$$

Thus $\phi(\tau)=\Theta_4(2\tau)$. The same Poisson calculation with a phase or shifted lattice gives $\Theta_4(-1/z)=\sqrt{-iz}\Theta_2(z)$ and $\Theta_2(-1/z)=\sqrt{-iz}\Theta_4(z)$. Translation gives $\Theta_4(z+2)=\Theta_4(z)$ and $\Theta_2(z-1)=e^{-\pi i/4}\Theta_2(z)$. These are [theta-constant inversion and translation laws](../../../../../../theta-constant-inversion-and-translation-laws.md).

Let $U\tau=\tau/(2\tau+1)$ and put $w=-1/z-1$, so $2U\tau=-1/w$. Raising the preceding identities to the eighth power removes all square-root and phase ambiguities:

$$
\Theta_4(2U\tau)^8=w^4\Theta_2(w)^8=w^4z^4\Theta_4(z)^8=(2\tau+1)^4\phi(\tau)^8.
$$

Also $\phi(\tau+1)^8=\phi(\tau)^8$. The given generators, including their negatives, therefore establish weight four for $\phi^8$ on $\Gamma_0(2)$, and weight $4k$ for $\phi^{8k}$.

The defining series is holomorphic and its expansion at infinity has no negative powers. At the other [modular cusp](../../../../../../cusp-of-a-modular-group.md),

$$
(\phi^8|_4S)(\tau)=\frac1{16}\Theta_2(\tau/2)^8.
$$

Writing $q_0=e^{\pi i\tau}$ gives $\Theta_2(\tau/2)=2q_0^{1/8}\sum_{n\ge0}q_0^{n(n+1)/2}$, so the right side begins $16q_0$ and is a holomorphic power series in $q_0$. Taking its $k$th power proves [modular cusp](../../../../../../cusp-of-a-modular-group.md) holomorphy for every $k>0$. Consequently

$$
\boxed{\phi^{8k}\in M_{4k}(\Gamma_0(2)).}
$$

The exponent in the shifted series is $n^2$, as printed in the PDF, not the corrupted exponent in the TeX aid.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
