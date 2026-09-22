<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat g(\xi)=\int_{\mathbb R}g(x)e^{-2\pi ix\xi}\,dx$. For $t>0$, completing the square in the [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
g_t(x)=e^{-\pi tx^2},\qquad \widehat g_t(\xi)=t^{-1/2}e^{-\pi\xi^2/t}.
$$

Both functions are rapidly decreasing, so the [Poisson summation formula](../../../../../poisson-summation-formula.md) applies:

$$
\sum_{n\in\mathbb Z}e^{-\pi tn^2}=t^{-1/2}\sum_{n\in\mathbb Z}e^{-\pi n^2/t}.
$$

In terms of the [Jacobi theta function](../../../../../jacobi-theta-function.md), this is $\vartheta(i/t)=\sqrt t\,\vartheta(it)$. The theta series converges locally uniformly in the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md), defining a [holomorphic function](../../../../../holomorphic-function.md). The branch of $\sqrt{-i\tau}$ with positive value at $\tau=it$ is holomorphic there, because $-i\tau$ lies in the right half-plane. Both sides of the proposed inversion identity are holomorphic; agreement on the positive imaginary axis and the [identity theorem](../../../../../identity-theorem.md) give

$$
\boxed{\vartheta(-1/\tau)=\sqrt{-i\tau}\,\vartheta(\tau).}
$$

Equivalently, the complex Gaussian has transform $(-i\tau)^{-1/2}\exp(-\pi i\xi^2/\tau)$, which produces the same identity directly by [Poisson summation](../../../../../poisson-summation-formula.md).

Put $\psi(t)=(\vartheta(it)-1)/2=\sum_{n\geq1}e^{-\pi n^2t}$. For $\operatorname{Re}s>1$, integrate term by term in its [Mellin transform](../../../../../mellin-transform.md):

$$
Z(s):=\int_0^\infty\psi(t)t^{s/2-1}\,dt
=\pi^{-s/2}\Gamma(s/2)\zeta(s).
$$

The [theta function](../../../../../theta-function.md) inversion gives

$$
\psi(t)=t^{-1/2}\psi(1/t)+\frac{t^{-1/2}-1}{2}.
$$

Split the integral at one. In the term containing $\psi(1/t)$ put $t=1/u$. The elementary remainder integral is

$$
\frac12\int_0^1\left(t^{(s-1)/2-1}-t^{s/2-1}\right)dt
=\frac1{s-1}-\frac1s.
$$

Thus the [pole-subtracted theta integral for the completed zeta function](../../../../../pole-subtracted-theta-integral-for-the-completed-zeta-function.md) is

$$
\boxed{Z(s)=\int_1^\infty\psi(t)\left(t^{s/2-1}+t^{(1-s)/2-1}\right)dt+\frac1{s-1}-\frac1s.}
$$

The integral is entire by exponential decay. This supplies a [meromorphic continuation](../../../../../meromorphic-continuation.md) with simple poles at zero and one, of residues $-1$ and $1$. The expression is unchanged by $s\mapsto1-s$, proving the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md)

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s).}
$$

The reflection and duplication identities $\Gamma(z)\Gamma(1-z)=\pi/\sin\pi z$ and $\Gamma(z)\Gamma(z+1/2)=2^{1-2z}\sqrt\pi\Gamma(2z)$ convert it to

$$
\boxed{\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s).}
$$

Multiplying $Z$ by $s(s-1)/2$ removes its two poles and yields the [Riemann xi function](../../../../../riemann-xi-function.md), which is an [entire function](../../../../../entire-function.md), satisfying $\xi(s)=\xi(1-s)$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 88](../../paper-88-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
