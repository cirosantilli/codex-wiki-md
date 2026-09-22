<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the integral with an explicit dummy time:

$$
X_t=M_t-\int_0^tZ_s^{-1}\,d\langle M,Z\rangle_s.
$$

On every compact time interval, strict positivity and continuity of $Z$ make its reciprocal locally bounded; the covariation has locally finite variation. Thus $X$ is a well-defined continuous semimartingale.

Apply the [Itô product rule](../../../../../ito-product-rule.md). Subtracting a finite-variation process does not change covariation, so $[Z,X]=[Z,M]$. The finite-variation terms cancel:

$$
\begin{aligned}
d(ZX)&=X\,dZ+Z\,dX+d[Z,X]\\
&=X\,dZ+Z\,dM-d[M,Z]+d[Z,M]\\
&=X\,dZ+Z\,dM.
\end{aligned}
$$

Thus $ZX$ is a local martingale under $\mathbb P$.

For the transfer step, choose stopping times increasing to the horizon that bound $X$, $M$, reciprocal $Z$, and the brackets needed for the stochastic integrals. For each such time $\sigma$, the same product calculation with $X^\sigma$ shows that $Z_tX_{t\wedge\sigma}$ is a true $\mathbb P$ martingale. The part after $\sigma$ is simply the bounded held value $X_\sigma$ times the density martingale. By the [Bayes formula for conditional expectation](../../../../../bayes-formula-for-conditional-expectation.md), for $s\leq t$,

$$
\mathbb E_{\mathbb Q}(X_{t\wedge\sigma}\mid\mathcal F_s)
=\frac{\mathbb E_{\mathbb P}(Z_tX_{t\wedge\sigma}\mid\mathcal F_s)}{Z_s}
=X_{s\wedge\sigma}.
$$

The stopping times exhaust the horizon also under $\mathbb Q\ll\mathbb P$. Hence **$X$ is a continuous $\mathbb Q$ local martingale**, proving this form of the [Girsanov theorem](../../../../../girsanov-theorem.md) without assuming a positive terminal density everywhere.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
