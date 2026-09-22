<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Start at $x=(x_1,\ldots,x_n)$ with all $x_i>0$, and let $\tau_i$ be the first zero of the $i$th coordinate. The orthant exit time is $T=\min_i\tau_i$. The coordinate processes are [independent](../../../../../../independent-random-variables.md), so

$$
\mathbb P_x(T>t)=\prod_{i=1}^n\mathbb P_{x_i}(\tau_i>t)
=\prod_{i=1}^n\left[2\Phi(x_i/\sqrt t)-1\right].
$$

Here the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) gives $\mathbb P_a(\tau\leq t)=2\mathbb P(B_t\leq-a)$; $\Phi$ is the [standard normal distribution](../../../../../../standard-normal-distribution.md) function. Since $\Phi(z)-1/2=z/\sqrt{2\pi}+o(z)$ as $z\to0$,

$$
\mathbb P_x(T>t)\sim(2/\pi)^{n/2}(x_1\cdots x_n)t^{-n/2}\quad(t\to\infty).
$$

The [tail integral formula for expectation](../../../../../../tail-integral-formula-for-expectation.md), $\mathbb E_xT=\int_0^\infty\mathbb P_x(T>t)dt$, has a bounded integrand on $(0,1)$ and converges at infinity exactly when $n/2>1$. Therefore the [Brownian exit-time expectation in an orthant](../../../../../../brownian-exit-time-expectation-in-an-orthant.md) gives

$$
\boxed{g_{D_1}=\infty,\qquad g_{D_2}=\infty,\qquad g_{D_3}<\infty\text{ everywhere in }D_3.}
$$

The divergence for $n=2$ is logarithmic; almost-sure finiteness of the exit time does not imply a finite [expectation](../../../../../../expected-value.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
