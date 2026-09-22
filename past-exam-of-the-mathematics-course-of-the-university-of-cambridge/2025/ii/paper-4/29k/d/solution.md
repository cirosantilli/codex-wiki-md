<h1 id="29k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathcal F_s=\sigma(W_r:0\leq r\leq s)$ and fix $c\in\mathbb R$. The martingale property between $s$ and $t$ gives

$$
\mathbb E[e^{cW_t}\mid\mathcal F_s]
=e^{cW_s}
+\frac{c^2}{2}\int_s^t
\mathbb E[e^{cW_r}\mid\mathcal F_s]\,dr.
$$

For fixed $s$, write the left-hand conditional expectation at time $t$ as $G(t)$. This integral equation has the unique solution

$$
G(t)=e^{cW_s}\exp\left(\frac{c^2}{2}(t-s)\right).
$$

Multiplication by the $\mathcal F_s$-measurable factor $e^{-cW_s}$ therefore yields the conditional moment-generating function

$$
\boxed{
\mathbb E[e^{c(W_t-W_s)}\mid\mathcal F_s]
=\exp\left(\frac{c^2}{2}(t-s)\right)}.
$$

This is the moment-generating function of $N(0,t-s)$ and is deterministic. Hence $W_t-W_s$ has that normal law conditionally on $\mathcal F_s$, and its conditional law does not depend on $\mathcal F_s$; the increment is therefore independent of the past.

The process starts at zero by assumption and has continuous paths. The independent centred Gaussian increments just obtained complete the definition of Brownian motion. This proves the [exponential test-function characterization of Brownian motion](../../../../../../exponential-test-function-characterization-of-brownian-motion.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
