<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Fourier transform](../../../../../fourier-transform.md) normalization $\widehat f(\xi)=\int_{\mathbb R}f(x)e^{-2\pi ix\xi}\,dx$. A precise version of the [Poisson summation formula](../../../../../poisson-summation-formula.md) is that, for every [Schwartz function](../../../../../schwartz-function.md) $f\in\mathcal S(\mathbb R)$,

$$
\boxed{\sum_{n\in\mathbb Z}f(n)=\sum_{m\in\mathbb Z}\widehat f(m).}
$$

Both series have [absolute convergence](../../../../../absolute-convergence.md). Here being a [Schwartz function](../../../../../schwartz-function.md) means being smooth with $\sup_x|x^a f^{(b)}(x)|<\infty$ for all nonnegative integers $a,b$. This hypothesis makes the sums and the termwise operations below legitimate; the formula is not being asserted for arbitrary integrable [functions](../../../../../function-split.md).

Form the [periodization of a Schwartz function](../../../../../periodization-of-a-schwartz-function.md) $P_f(x)=\sum_n f(x+n)$. Every differentiated series has [uniform convergence](../../../../../uniform-convergence.md) on $[0,1]$, by rapid decay, so $P_f$ is a smooth [periodic function](../../../../../periodic-function.md) of period one. Its $m$th [Fourier coefficient](../../../../../fourier-coefficient.md) is

$$
\int_0^1P_f(x)e^{-2\pi imx}\,dx
=\sum_n\int_n^{n+1}f(u)e^{-2\pi imu}\,du=\widehat f(m).
$$

The interchange follows from [absolute convergence](../../../../../absolute-convergence.md) uniformly on this interval. [Integration by parts](../../../../../integration-by-parts.md) shows that these [Fourier coefficients](../../../../../fourier-coefficient.md) decrease faster than every inverse power of $|m|$. Thus the [Fourier series](../../../../../fourier-series-split.md) converges absolutely and uniformly to $P_f$; for example the standard convergence theorem for twice continuously differentiable [periodic functions](../../../../../periodic-function.md) applies. Evaluating at zero proves the [Poisson summation formula](../../../../../poisson-summation-formula.md).

For $t>0$, scaling the given Gaussian [Fourier transform](../../../../../fourier-transform.md) gives

$$
\widehat{e^{-\pi t x^2}}(\xi)=t^{-1/2}e^{-\pi\xi^2/t}.
$$

Applying the [Poisson summation formula](../../../../../poisson-summation-formula.md) gives the real-parameter [Jacobi theta function](../../../../../jacobi-theta-function.md) transformation

$$
\boxed{\theta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t}=t^{-1/2}\theta(1/t).}
$$

For $\operatorname{Re}s>1$, termwise application of the [Mellin transform](../../../../../mellin-transform.md) is justified by integrating absolute values and gives

$$
\Lambda(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\frac12\int_0^\infty(\theta(t)-1)t^{s/2-1}\,dt.
$$

Each positive $n$ contributes $\Gamma(s/2)(\pi n^2)^{-s/2}$, and the factor one half removes the equal positive and negative terms. This is the [Mellin representation of the completed Riemann zeta function](../../../../../mellin-representation-of-the-completed-riemann-zeta-function.md).

Split the integral at one. On $(0,1)$, the [Jacobi theta function](../../../../../jacobi-theta-function.md) transformation writes $\theta(t)-1=t^{-1/2}-1+t^{-1/2}(\theta(1/t)-1)$. Integrating the first two terms and substituting $u=1/t$ in the third yields the [pole-subtracted theta integral for the completed zeta function](../../../../../pole-subtracted-theta-integral-for-the-completed-zeta-function.md):

$$
\Lambda(s)=\frac1{s-1}-\frac1s+
\frac12\int_1^\infty(\theta(t)-1)
\left(t^{s/2-1}+t^{(1-s)/2-1}\right)\,dt.
$$

The remaining integral is an [entire function](../../../../../entire-function.md) of $s$: $\theta(t)-1=O(e^{-\pi t})$, and on each compact set of $s$ this exponential dominates all powers of $t$ and all factors arising from differentiation. It therefore supplies a [meromorphic continuation](../../../../../meromorphic-continuation.md) of $\Lambda$ to the whole plane, with simple [poles](../../../../../pole.md) at one and zero, of residues $1$ and $-1$, respectively. Its expression is unchanged by $s\mapsto1-s$.

The reciprocal [Gamma function](../../../../../gamma-function.md) is entire, with simple zeros at its nonpositive integer arguments. Consequently

$$
\zeta(s)=\pi^{s/2}\Gamma(s/2)^{-1}\Lambda(s)
$$

is holomorphic everywhere except for a simple [pole](../../../../../pole.md) at $s=1$, of residue one. The apparent [pole](../../../../../pole.md) at $s=0$ cancels; in fact $\Gamma(s/2)^{-1}\sim s/2$ gives $\zeta(0)=-1/2$. This proves the [analytic continuation](../../../../../analytic-continuation.md) of the [Riemann zeta function](../../../../../riemann-zeta-function.md). The completed [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) is

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s).}
$$

These are equalities of [meromorphic functions](../../../../../meromorphic-function.md); at apparent singularities they are interpreted by continuation. Equivalently, $\xi(s)=\tfrac12s(s-1)\Lambda(s)$ is an [entire function](../../../../../entire-function.md) with $\xi(s)=\xi(1-s)$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 137](../../paper-137-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
