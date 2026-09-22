<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**No [weakly stationary process](../../../../../../../weakly-stationary-process.md) solves the model with nondegenerate noise.** Iteration would give

$$
X_t-X_{t-m}=\sum_{j=0}^{m-1}\varepsilon_{t-j},\qquad \operatorname{Var}(X_t-X_{t-m})=m\sigma^2.
$$

For a [weakly stationary process](../../../../../../../weakly-stationary-process.md) with finite [variance](../../../../../../../variance-split.md) $V$, the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) instead gives $\operatorname{Var}(X_t-X_{t-m})=2V-2\gamma(m)\leq4V$. These two bounds contradict each other for large $m$. This argument does not assume that $X_{t-m}$ is independent of the intervening noise, so it excludes noncausal solutions too. The corresponding [unit-root autoregressive process](../../../../../../../unit-root-autoregressive-process.md) has persistent [random walk](../../../../../../../random-walk.md) behavior rather than stationary fluctuations.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
