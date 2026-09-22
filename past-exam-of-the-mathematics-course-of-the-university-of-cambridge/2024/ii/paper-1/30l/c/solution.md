<h1 id="30l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $P$ be the state-by-asset [matrix](../../../../../../matrix.md) of discounted gains and identify $Y$ with its state [vector](../../../../../../vector.md). Fix $q^0\in\mathcal Q$. If $q\geq0$, $P^Tq=0$, and $q\ne0$, then

$$
q_\varepsilon=\frac{q+\varepsilon q^0}{\sum_i(q_i+\varepsilon q_i^0)}
$$

belongs to $\mathcal Q$. The assumption and passage to the [limit](../../../../../../limit-of-a-function.md) imply $q^TY\geq0$ for every nonnegative $q\in\ker P^T$.

The [finite-state superhedging alternative](../../../../../../finite-state-superhedging-alternative.md) now gives $\theta$ with

$$
Y-P\theta\geq0.
$$

This residual cannot vanish identically, since then every $Q\in\mathcal Q$ would have $E_QY=q^TP\theta=0$. Hence it is strictly positive in at least one state, which has positive physical probability. This is the required inequality.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30L](../../30l.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
