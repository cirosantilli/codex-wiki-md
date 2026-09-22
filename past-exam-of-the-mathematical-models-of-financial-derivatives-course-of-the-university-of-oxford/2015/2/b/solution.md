<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [Itô's formula](../../../../ito-s-lemma.md) to the [logarithm](../../../../logarithm.md) of the positive [geometric Brownian motion](../../../../geometric-brownian-motion.md). The quadratic-variation correction gives

$$
d\log S_t=(r-\sigma^2/2)dt+\sigma dW_t.
$$

Integrating yields

$$
\boxed{S_T=S_t\exp\!\left[(r-\sigma^2/2)(T-t)+\sigma(W_T-W_t)\right].}
$$

The increment is a [Gaussian random variable](../../../../gaussian-random-variable.md) with [variance](../../../../variance-split.md) $T-t$, independent of current information. Writing it as $W_\tau$ means a fresh future [Brownian motion](../../../../brownian-motion-split.md) $\widetilde W_v=W_{t+v}-W_t$, evaluated at $\tau$; it need not equal the original process at time $T-t$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
