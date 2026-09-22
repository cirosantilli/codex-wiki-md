<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $Q_t=\langle M,M\rangle_t$ and $F(x,q)=e^{\sigma x-\sigma^2q/2}$. In the two-variable [Itô formula](../../../../ito-s-lemma.md), $Q$ has finite variation, while the only nonzero quadratic term is $d\langle M\rangle=dQ$. Therefore

$$
dF(M_t,Q_t)=\sigma F\,dM_t-\tfrac12\sigma^2F\,dQ_t
+\tfrac12\sigma^2F\,dQ_t=\sigma F\,dM_t.
$$

This proves the [stochastic exponential](../../../../doleans-dade-exponential.md) solves the equation. Its initial value is $e^{\sigma M_0}$; no normalization $M_0=0$ was stipulated.

The resulting process is initially a [continuous local martingale](../../../../continuous-local-martingale.md). Since $Q_t\geq0$ and $|M_t|<C$,

$$
0<Z_t=e^{\sigma M_t-\sigma^2Q_t/2}\leq e^{|\sigma|C}.
$$

A bounded local martingale is a true [martingale](../../../../martingale-split.md): apply the martingale identity to a localizing sequence and use [dominated convergence](../../../../dominated-convergence-theorem.md) in conditional expectations. The deterministic bound works on every finite horizon, proving **$Z$ is a martingale on every $[0,T]$**. The bound on $Q$ also gives a positive deterministic lower bound $e^{-|\sigma|C-\sigma^2C/2}$, although the upper bound already proves the martingale assertion.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
