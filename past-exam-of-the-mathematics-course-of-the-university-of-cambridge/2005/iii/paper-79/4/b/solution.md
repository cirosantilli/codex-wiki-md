<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First assume the usual diffusion regime $\gamma>0$, with $U$ real; the complex-diffusion extension is described below. Substitution of a global [normal mode](../../../../../../normal-mode.md) gives

$$
\gamma a''-Ua'+(\mu_0-\nu\varepsilon^2x^2+i\omega_G)a=0.
$$

Set $a=e^{Ux/(2\gamma)}b$ to remove the first [derivative](../../../../../../derivative.md), then put $\xi=\sqrt\varepsilon(\nu/\gamma)^{1/4}x$. The resulting oscillator equation is

$$
\boxed{b_{\xi\xi}+(\Lambda-\xi^2)b=0,\qquad \Lambda=\frac{\mu_0-U^2/(4\gamma)+i\omega_G}{\varepsilon\sqrt{\gamma\nu}}.}
$$

Writing $b=e^{-\xi^2/2}H(\xi)$ gives the [Hermite differential equation](../../../../../../hermite-differential-equation.md), $H''-2\xi H'+(\Lambda-1)H=0$. For a [power series](../../../../../../power-series.md) $H=\sum_{j\geq0}c_j\xi^j$, its recurrence is

$$
c_{j+2}=\frac{2j+1-\Lambda}{(j+2)(j+1)}c_j.
$$

Termination at degree $n$ requires $\Lambda=2n+1$. If it does not terminate in the appropriate parity, the series has a growing Gaussian component at one infinity; the solution decaying at one end then fails at the other. The [Hermite oscillator quantization](../../../../../../hermite-oscillator-quantization.md) can also be seen from the self-adjoint operator $-d^2/d\xi^2+\xi^2$, whose square-integrable [eigenfunctions](../../../../../../eigenfunction.md) are the [Hermite functions](../../../../../../hermite-function.md). Their spectrum is $2n+1$ with $n=0,1,2,\ldots$. The ground state $H_0=1$ shows that the paper's phrase “positive integer” must include zero.

The [global modes of a quadratically confined Ginzburg-Landau equation](../../../../../../global-modes-of-a-quadratically-confined-ginzburg-landau-equation.md) are therefore

$$
\boxed{\omega_{G,n}=i\left[\mu_0-\frac{U^2}{4\gamma}-(2n+1)\varepsilon\sqrt{\gamma\nu}\right],\qquad n=0,1,2,\ldots.}
$$

Their spatial functions are proportional to $e^{Ux/(2\gamma)}e^{-\xi^2/2}H_n(\xi)$; the quadratic Gaussian decay dominates the linear drift factor at both infinities. For real coefficients, the most dangerous mode is $n=0$. The system has [global hydrodynamic instability](../../../../../../global-hydrodynamic-instability.md) precisely when

$$
\boxed{\mu_0>\frac{U^2}{4\gamma}+\varepsilon\sqrt{\gamma\nu}.}
$$

Equality is marginal and smaller $\mu_0$ gives decay of all these modes. The finite-width confinement correction explains why a locally absolutely unstable region need not immediately support a growing global mode.

If complex diffusion is intended, impose the parabolic condition $\operatorname{Re}\gamma>0$ and choose $\sqrt{\nu/\gamma}$ with positive real part. The same formulas continue along the rotated $\xi$ ray, with the corresponding branch of $\sqrt{\gamma\nu}$; instability is determined by the real part of the square bracket. Arbitrary constant $\gamma$, especially negative diffusion, does not justify the asserted whole-line Hermite decay or a well-posed evolution.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
