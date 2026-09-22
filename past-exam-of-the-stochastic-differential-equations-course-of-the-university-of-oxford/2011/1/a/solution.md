<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Bessel process](../../../../bessel-process.md) is stopped in the compact interval $[\alpha,\beta]$, where its drift and diffusion coefficients are bounded. In particular its stopped stochastic integral has expectation zero on every finite time interval.

For $k>1$, taking expectations in the stopped equation gives

$$
\mathbb E Y_t-1=\frac{k-1}{2}\mathbb E\int_0^{t\wedge\tau}\frac{ds}{y_s}
\geq\frac{k-1}{2\beta}\mathbb E(t\wedge\tau).
$$

Since $Y_t\leq\beta$, this bounds $\mathbb E(t\wedge\tau)$ uniformly in $t$. For $k<1$, the same argument with $1-\mathbb E Y_t$ gives $\mathbb E(t\wedge\tau)\leq2\beta(1-\alpha)/(1-k)$.

If $k=1$, the stopped process is a stopped Brownian motion. [Itô's formula](../../../../ito-s-lemma.md) gives $\mathbb E(Y_t-1)^2=\mathbb E(t\wedge\tau)$, which is at most $\max\{(1-\alpha)^2,(\beta-1)^2\}$. Thus in every case the [monotone convergence theorem](../../../../monotone-convergence-theorem.md) gives $\mathbb E\tau<\infty$, so $\tau<\infty$ almost surely. By path continuity its value at exit is one of the two endpoints. They are disjoint possibilities, hence

$$
\boxed{\mathbb P(y_\tau=\alpha)+\mathbb P(y_\tau=\beta)=1.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the stochastic differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations course of the University of Oxford](../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
