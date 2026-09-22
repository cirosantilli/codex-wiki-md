<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $e(t)=e^{2\pi it}$ and the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat f(\xi)=\int_{\mathbb R}f(x)e(-x\xi)\,dx$, initially for an [integrable function](../../../../../lebesgue-integrable-function.md). For the interval [indicator function](../../../../../indicator-function.md), direct integration gives

$$
\widehat{1_{[0,1]}}(\xi)=\begin{cases}(1-e(-\xi))/(2\pi i\xi),&\xi\ne0,\\1,&\xi=0.\end{cases}
$$

The integral bound is one, and the displayed numerator has modulus at most two. By the [convolution theorem](../../../../../convolution-theorem.md), the [Fourier transform](../../../../../fourier-transform.md) of the $m$-fold [convolution](../../../../../convolution.md) is its $m$th power. Thus the [Fourier decay of repeated interval convolutions](../../../../../fourier-decay-of-repeated-interval-convolutions.md) gives

$$
\boxed{|\widehat f(\xi)|\le\min(1,(\pi|\xi|)^{-m})\ll\min(1,|\xi|^{-m}).}
$$

At zero, interpret the second term of the minimum as infinity.

The [Schwartz space](../../../../../schwartz-space.md) $\mathcal S(\mathbb R)$ consists of [smooth functions](../../../../../smooth-function.md) for which every [Schwartz seminorm](../../../../../schwartz-seminorm.md) $\sup_x|x^a f^{(b)}(x)|$ is finite, for nonnegative integers $a,b$. [Differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) and [integration by parts](../../../../../integration-by-parts.md) give

$$
\widehat f^{(b)}(\xi)=\widehat{(-2\pi ix)^bf}(\xi),\qquad
(2\pi i\xi)^a\widehat f^{(b)}(\xi)=\widehat{\frac{d^a}{dx^a}\bigl((-2\pi ix)^bf(x)\bigr)}(\xi).
$$

All differentiated integrands are [integrable](../../../../../integrability.md), and their boundary terms vanish because of rapid decay. The last transform is bounded by its integrand's $L^1$ [norm](../../../../../norm.md). The same argument applies at every derivative order, so $\widehat f\in\mathcal S(\mathbb R)$.

For $f\in\mathcal S(\mathbb R)$, the [Poisson summation formula](../../../../../poisson-summation-formula.md) is

$$
\boxed{\sum_{n\in\mathbb Z}f(n)=\sum_{k\in\mathbb Z}\widehat f(k).}
$$

To prove it, form the [periodization of a Schwartz function](../../../../../periodization-of-a-schwartz-function.md) $F(x)=\sum_n f(x+n)$. Rapid decay gives [uniform convergence](../../../../../uniform-convergence.md) of this series and of every differentiated series on $[0,1]$, so $F$ is a smooth [periodic function](../../../../../periodic-function.md). Its [Fourier coefficients](../../../../../fourier-coefficient.md) are

$$
\int_0^1F(x)e(-kx)\,dx=\sum_n\int_n^{n+1}f(u)e(-ku)\,du=\widehat f(k).
$$

The series $\sum_k\widehat f(k)e(kx)$ converges absolutely and uniformly. Its [Fourier coefficients](../../../../../fourier-coefficient.md) equal those of $F$. The uniqueness theorem for [Fourier series](../../../../../fourier-series-split.md) says that two [integrable functions](../../../../../lebesgue-integrable-function.md) with the same coefficients agree almost everywhere; as both functions here are continuous, they agree everywhere. Evaluating at zero proves [Poisson summation](../../../../../poisson-summation-formula.md).

The [Gaussian Fourier transform](../../../../../fourier-transform-of-a-gaussian.md) of $e^{-\pi tx^2}$, $t>0$, is $t^{-1/2}e^{-\pi\xi^2/t}$. Apply [Poisson summation](../../../../../poisson-summation-formula.md) to obtain the transformation of the [Jacobi theta function](../../../../../jacobi-theta-function.md)

$$
\vartheta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t},\qquad \vartheta(t)=t^{-1/2}\vartheta(1/t).
$$

For $\Re s>1$, termwise integration in the [Mellin transform](../../../../../mellin-transform.md) gives the [Mellin representation of the completed Riemann zeta function](../../../../../mellin-representation-of-the-completed-riemann-zeta-function.md)

$$
\Lambda(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)=\frac12\int_0^\infty(\vartheta(t)-1)t^{s/2-1}\,dt.
$$

Split at one and substitute $t=1/u$ in the lower integral. The theta transformation gives

$$
\Lambda(s)=\frac1{s-1}-\frac1s+\frac12\int_1^\infty(\vartheta(t)-1)\bigl(t^{s/2-1}+t^{(1-s)/2-1}\bigr)\,dt.
$$

The integral is an [entire function](../../../../../entire-function.md) of $s$, since $\vartheta(t)-1$ decays exponentially. This [pole-subtracted theta integral for the completed zeta function](../../../../../pole-subtracted-theta-integral-for-the-completed-zeta-function.md) supplies a [meromorphic continuation](../../../../../meromorphic-continuation.md) with simple [poles](../../../../../pole.md) at zero and one. Both the rational term and the integral are unchanged by $s\mapsto1-s$, proving the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md)

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s).}
$$

Equivalently the [Riemann xi function](../../../../../riemann-xi-function.md) $\xi(s)=\frac12s(s-1)\Lambda(s)$ is [entire](../../../../../entire-function.md) and satisfies $\xi(s)=\xi(1-s)$. The reflection and duplication identities for the [Gamma function](../../../../../gamma-function.md) also give $\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s)$ by [meromorphic continuation](../../../../../meromorphic-continuation.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
