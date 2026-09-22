<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Fourier transform](../../../../../fourier-transform-split.md) convention $\widehat f(\xi)=\int_{\mathbb R}f(x)e^{-ix\xi}\,dx$, with complex-linear [distribution](../../../../../distribution-mathematical-analysis.md) pairings throughout. The [Riemann-Lebesgue lemma](../../../../../riemann-lebesgue-lemma.md) says that, for an [integrable function](../../../../../lebesgue-integrable-function.md) $f\in L^1(\mathbb R)$, its [Fourier transform](../../../../../fourier-transform-split.md) is continuous and tends to zero as $|\xi|\to\infty$. It also satisfies $\|\widehat f\|_\infty\leq\|f\|_1$. The product rule, or [convolution theorem](../../../../../convolution-theorem.md), is

$$
\boxed{\widehat{f*g}=\widehat f\,\widehat g\qquad(f,g\in L^1(\mathbb R)).}
$$

Here $(f*g)(x)=\int f(y)g(x-y)\,dy$ belongs to $L^1(\mathbb R)$ by [Tonelli's theorem](../../../../../tonelli-theorem.md), and [Fubini's theorem](../../../../../fubini-s-theorem.md) proves the displayed identity. The companion [Fourier product formula](../../../../../fourier-product-formula.md), for [Schwartz functions](../../../../../schwartz-function.md), is $\widehat{fg}=(2\pi)^{-1}\widehat f*\widehat g$.

A [Schwartz function](../../../../../schwartz-function.md) is a [smooth function](../../../../../smooth-function.md) $\phi:\mathbb R\to\mathbb C$ for which every [Schwartz seminorm](../../../../../schwartz-seminorm.md)

$$
p_{m,n}(\phi):=\sup_{x\in\mathbb R}|x^m\phi^{(n)}(x)|,\qquad m,n\in\{0,1,2,\ldots\},
$$

is finite. These [seminorms](../../../../../seminorm.md) define the topology of the [Schwartz space](../../../../../schwartz-space.md) $\mathcal S(\mathbb R)$. In particular,

$$
|\phi(x)|\leq\frac{p_{0,0}(\phi)+p_{2,0}(\phi)}{1+x^2},\qquad
\boxed{\|\phi\|_1\leq\pi\bigl(p_{0,0}(\phi)+p_{2,0}(\phi)\bigr)<\infty.}
$$

Thus every [Schwartz function](../../../../../schwartz-function.md) is an [integrable function](../../../../../lebesgue-integrable-function.md).

The [Fourier bounds for Schwartz functions](../../../../../fourier-bounds-for-schwartz-functions.md) assert that each [Schwartz seminorm](../../../../../schwartz-seminorm.md) of $\widehat\phi$ is bounded by finitely many [Schwartz seminorms](../../../../../schwartz-seminorm.md) of $\phi$. Explicitly, [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) and [integration by parts](../../../../../integration-by-parts.md) give

$$
\xi^m\partial_\xi^n\widehat\phi(\xi)
=i^{-m}\mathcal F\!\left[\partial_x^m\bigl((-ix)^n\phi\bigr)\right](\xi),
$$

so the [generalized Leibniz rule](../../../../../generalized-leibniz-rule.md) and the preceding integrability estimate give

$$
\boxed{p_{m,n}(\widehat\phi)
\leq\pi\sum_{j=0}^{\min(m,n)}\binom mj\frac{n!}{(n-j)!}
\bigl(p_{n-j,m-j}(\phi)+p_{n-j+2,m-j}(\phi)\bigr).}
$$

In particular the [Fourier transform](../../../../../fourier-transform-split.md) maps the [Schwartz space](../../../../../schwartz-space.md) continuously into itself.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
