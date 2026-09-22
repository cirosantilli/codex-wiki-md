<h1 id="17b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator.md), the [Time-independent Schrödinger equation](../../../../../../time-independent-schrodinger-equation.md) is

$$
-\frac{\hbar^2}{2m}\psi''+\frac12m\omega^2x^2\psi=E\psi,
$$

with $m,\omega,\hbar>0$. The given dimensionless coordinate yields $\psi_{\xi\xi}+(2E/(\hbar\omega)-\xi^2)\psi=0$. Substituting the Gaussian factor gives

$$
f''-2\xi f'+\left(\frac{2E}{\hbar\omega}-1\right)f=0.
$$

By the supplied normalizability fact, $f$ is a nonzero polynomial. If its degree is $n$, comparison of the leading coefficient forces $2E/(\hbar\omega)-1=2n$. Conversely, at this value the coefficient recurrence

$$
a_{j+2}=\frac{2j-2n}{(j+2)(j+1)}a_j
$$

produces a degree-$n$ polynomial with parity $n$: start with a nonzero constant for even $n$ or a nonzero linear coefficient for odd $n$, and the recurrence terminates at degree $n$. This is a multiple of the [Hermite polynomial](../../../../../../hermite-polynomial.md). Its product with the Gaussian is square integrable and can be normalized. Therefore all and only the allowed energies are

$$
\boxed{E_n=\left(n+\frac12\right)\hbar\omega,\qquad n=0,1,2,\ldots.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17B](../../17b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
