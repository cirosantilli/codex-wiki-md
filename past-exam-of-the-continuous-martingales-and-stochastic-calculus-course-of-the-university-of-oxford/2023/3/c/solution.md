<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $f(y)=|y|$ away from zero. Its first and second [partial derivatives](../../../../partial-derivative.md) are

$$
\partial_kf(y)=\frac{y_k}{|y|},\qquad
\partial_{jk}f(y)=\frac{\delta_{jk}}{|y|}-\frac{y_jy_k}{|y|^3}.
$$

Thus its [Laplace operator](../../../../laplace-operator.md) is $\Delta f(y)=(n-1)/|y|$. The [quadratic covariations](../../../../quadratic-covariation.md) of the [independent](../../../../independent-random-variables.md) Brownian coordinates satisfy $d[B_j,B_k]_s=\delta_{jk}ds$. The stopped [Itô formula](../../../../ito-s-lemma.md) therefore gives

$$
\boxed{X_{t\wedge\tau}=|x|+\frac{n-1}{2}\int_0^{t\wedge\tau}\frac{ds}{X_s}
+\sum_{k=1}^n\int_0^{t\wedge\tau}\frac{B_k(s)}{X_s}\,dB_k(s).}
$$

For $t<\tau$, this is the required integral representation.

To identify the driving [Brownian motion](../../../../brownian-motion-split.md), the stopped stochastic term alone is insufficient: its [quadratic variation](../../../../quadratic-variation.md) is $t\wedge\tau$. Extend its unit direction after exit. Define a vector [predictable process](../../../../predictable-process.md) $u(s)$ by

$$
u(s)=\begin{cases}B(s)/X_s,&s\leq\tau,\\(1,0,\ldots,0),&s>\tau,\end{cases}
\qquad
W_t=\sum_{k=1}^n\int_0^tu_k(s)\,dB_k(s).
$$

Predictability follows from the continuous adapted direction before stopping and the left-continuous adapted indicator $\mathbf1_{\{s\leq\tau\}}$. This $W$ is a zero-starting [continuous martingale](../../../../continuous-martingale.md), and

$$
[W]_t=\int_0^t\sum_{k=1}^nu_k(s)^2ds=t.
$$

The [Lévy characterization of Brownian motion](../../../../levy-characterization-of-brownian-motion.md) identifies $W$ as a one-dimensional [Brownian motion](../../../../brownian-motion-split.md). Before $\tau$, the preceding representation becomes the [stochastic differential equation](../../../../stochastic-differential-equation.md) of the dimension-$n$ [Bessel process](../../../../bessel-process.md):

$$
\boxed{dX_t=\frac{n-1}{2X_t}\,dt+dW_t\qquad(t<\tau).}
$$

The fully stopped equation has both integrals stopped at $\tau$.

For $n=2$, apply the one-dimensional [Itô formula](../../../../ito-s-lemma.md) to the [logarithm](../../../../logarithm.md). Before $\tau$, $d[X]_t=dt$, so the two drift terms cancel:

$$
d\log X_t=\frac1{X_t}\left(\frac1{2X_t}\,dt+dW_t\right)
-\frac1{2X_t^2}\,dt=\frac1{X_t}\,dW_t.
$$

Consequently,

$$
\boxed{\log X_{t\wedge\tau}=\log|x|+\int_0^{t\wedge\tau}\frac{dW_s}{X_s}
\quad\text{is a bounded martingale}.}
$$

Indeed $X_s\geq r$ before stopping, so the [Itô isometry](../../../../ito-isometry.md) bounds the stochastic term's second [moment](../../../../moment.md) by $t/r^2$, and $\log X_{t\wedge\tau}\in[\log r,\log R]$. This is the [martingale](../../../../martingale-split.md) assertion under the paper's standing stopping assumption. Without stopping, the same calculation establishes only a [local martingale](../../../../local-martingale.md); the stopped qualification is essential for the stated argument.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../split.md)
5. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
