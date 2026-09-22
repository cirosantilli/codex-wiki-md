<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $X,Y$ be two continuous solutions on the same [filtered probability space](../../../../../../filtered-probability-space.md), driven by the same [Brownian motion](../../../../../../brownian-motion-split.md) and with $X_0=Y_0$ [almost surely](../../../../../../almost-sure-convergence.md). Write $D=X-Y$ and choose a common [Lipschitz constant](../../../../../../lipschitz-constant.md) $L$ for $b,\sigma$. Introduce the [stopping time](../../../../../../stopping-time.md) $\tau_n=\inf\{t\geq0:|X_t|+|Y_t|\geq n\}$. On $\{\tau_n=0\}$ the stopped difference is zero; before $\tau_n$, both coefficients and the difference are bounded.

The [Itô formula](../../../../../../ito-s-lemma.md) and the zero [expectation](../../../../../../expected-value.md) of the stopped [square-integrable](../../../../../../square-integrable-function.md) [Itô integral](../../../../../../ito-integral.md) yield

$$
\begin{aligned}
\mathbb E D_{t\wedge\tau_n}^2
&=\mathbb E\int_0^t\mathbf1_{\{s<\tau_n\}}\left(2D_s(b(X_s)-b(Y_s))+(\sigma(X_s)-\sigma(Y_s))^2\right)ds\\
&\leq(2L+L^2)\int_0^t\mathbb E D_{s\wedge\tau_n}^2\,ds.
\end{aligned}
$$

The [Gronwall inequality](../../../../../../gronwall-inequality.md) implies $\mathbb ED_{t\wedge\tau_n}^2=0$. Continuous solution paths are bounded on each compact time interval, so $\tau_n\uparrow\infty$ [almost surely](../../../../../../almost-sure-convergence.md). Letting $n\to\infty$ proves $X_t=Y_t$ [almost surely](../../../../../../almost-sure-convergence.md) at each fixed time, and a countable dense set of times together with continuity gives [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md). Therefore **the [stochastic differential equation](../../../../../../stochastic-differential-equation.md) has [pathwise uniqueness](../../../../../../pathwise-uniqueness.md).**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
