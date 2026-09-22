<h1 id="30e/solution">Solution</h1>

↑ **Parent:** [30E](../30e.md)

Write $(\phi_\varepsilon*f)(x)=\int\phi(y)f(x-\varepsilon y)\,dy$. Since $\int\phi=1$,

$$
|(\phi_\varepsilon*f)(x)-f(x)|\leq\int|\phi(y)|\,|f(x-\varepsilon y)-f(x)|\,dy.
$$

A [Schwartz function](../../../../../schwartz-function.md) is bounded and [uniformly continuous](../../../../../uniform-continuity.md). Given a tolerance, first choose $R$ so the tail integral of $|\phi|$ is small. On $|y|\leq R$, [uniform continuity](../../../../../uniform-continuity.md) makes the difference uniformly small for every $x$ when $\varepsilon R$ is small. On the tail it is bounded by $2\|f\|_\infty$. This proves **[uniform convergence](../../../../../uniform-convergence.md)**, without assuming $\phi\geq0$, and is the [approximate identity](../../../../../approximate-identity.md) argument.

For the radial regularization of the three-dimensional [fundamental solution of the Laplace equation](../../../../../fundamental-solution-of-the-laplace-equation.md), direct differentiation gives

$$
-\Delta N_\varepsilon(x)=\frac{3\varepsilon^2}{4\pi(|x|^2+\varepsilon^2)^{5/2}}=\varepsilon^{-3}\phi(x/\varepsilon),\qquad\phi(x)=\frac3{4\pi}(1+|x|^2)^{-5/2}.
$$

The radial integral is $\int\phi=3\int_0^\infty r^2(1+r^2)^{-5/2}\,dr=1$. This even [approximate identity](../../../../../approximate-identity.md) therefore gives $\int(-\Delta N_\varepsilon)f\to f(0)$ for $f\in\mathcal S(\mathbb R^3)$.

The function $N=1/(4\pi|x|)$ is locally integrable and determines a [tempered distribution](../../../../../tempered-distribution.md). We have $0<N_\varepsilon\leq N$, and $N|\Delta f|$ is integrable near zero and infinity for a Schwartz test function. Integration by parts and the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) give

$$
\langle-\Delta N,f\rangle=\lim_{\varepsilon\downarrow0}\int N_\varepsilon(-\Delta f)=\lim_{\varepsilon\downarrow0}\int(-\Delta N_\varepsilon)f=f(0).
$$

Thus **$-\Delta N=\delta_0$**, proving that $N$ is a [fundamental solution of a linear differential operator](../../../../../fundamental-solution-of-a-linear-differential-operator.md). In this last part the test-function space is $\mathcal S(\mathbb R^3)$; the printed $\mathbb R^n$ in the three-dimensional integral is understood with $n=3$.

## ↑ Ancestors (10)

1. [30E](../30e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
