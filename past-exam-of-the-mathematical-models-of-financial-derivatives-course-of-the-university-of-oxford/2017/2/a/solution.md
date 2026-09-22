<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a positive starting value, [Itô's formula](../../../../ito-s-lemma.md) applied to $\log S_u$ gives $d\log S_u=(\mu-\sigma^2/2)du+\sigma dW_u$. Hence the [geometric Brownian motion](../../../../geometric-brownian-motion.md) is

$$
\boxed{S_T=S\exp\!\left[(\mu-\sigma^2/2)\tau+\sigma(W_T-W_t)\right].}
$$

The future [Brownian increment](../../../../brownian-increment.md) $W_T-W_t$ is independent of $\mathcal F_t$ and has [normal distribution](../../../../normal-distribution.md) $N(0,\tau)$. If $\widetilde W_v=W_{t+v}-W_t$, then $\widetilde W$ is a fresh [Brownian motion](../../../../brownian-motion-split.md) and the increment is exactly $\widetilde W_\tau$. This specifies the meaning of the paper's abbreviated $W_\tau$; the original process value $W_{T-t}$ is not generally that future increment. The [stochastic exponential](../../../../doleans-dade-exponential.md) solution also verifies positivity for $S>0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
