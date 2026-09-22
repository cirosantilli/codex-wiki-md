<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start both systems from zero and compare their times to reach half of their **own** [steady concentrations](../../../../steady-state.md). Without regulation,

$$
Y(t)=\frac\beta\alpha(1-e^{-\alpha t}),\qquad
Y_{\rm st}^{(0)}=\frac\beta\alpha,\qquad T_{1/2}^{(0)}=\frac{\log2}{\alpha}.
$$

In the strong [logic approximation for gene regulation](../../../../logic-approximation-for-gene-regulation.md), [production](../../../../gene-expression.md) is initially fully on and the [concentration](../../../../concentration.md) rises towards the repression threshold. The regulated level is pinned near $Y_{\rm st}\simeq K$, so it reaches $K/2$ before switching:

$$
\boxed{T_{1/2}^{\rm logic}=-\frac1\alpha\log\left(1-\frac{\alpha K}{2\beta}\right),\qquad
\frac{T_{1/2}^{\rm logic}}{T_{1/2}^{(0)}}=
\frac{-\log[1-\alpha K/(2\beta)]}{\log2}
\simeq\frac{\alpha K}{2\beta\log2}\ll1.}
$$

The faster relative response comes from allowing high initial [production](../../../../gene-expression.md) while keeping the final abundance low. [Negative autoregulation](../../../../negative-autoregulation.md) can reduce response delays and [sensitivity](../../../../sensitivity-analysis.md) to [production](../../../../gene-expression.md) fluctuations, and can reduce unnecessary accumulation of a [protein](../../../../protein-split.md). It does not suppress every possible noise source at every frequency.

A perfectly discontinuous on/off right-hand side has a threshold-switching ambiguity rather than an ordinary smooth equilibrium at $K$. Here threshold pinning means the limiting rapid-switching or steep smooth-response idealization. A continuous repression law resolves that idealization. Comparing half of the same prescribed [concentration](../../../../concentration.md), rather than half of each model's final [concentration](../../../../concentration.md), would be a different response-time comparison.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
