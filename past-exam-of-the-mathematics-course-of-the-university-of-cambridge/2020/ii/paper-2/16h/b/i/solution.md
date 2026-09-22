<h1 id="16h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Godel completeness theorem](../../../../../../../godel-s-completeness-theorem.md) says that for every first-order theory $\Gamma$ and sentence $\varphi$,

$$
\Gamma\models\varphi\quad\Longrightarrow\quad\Gamma\vdash\varphi.
$$

Together with [soundness](../../../../../../../soundness-theorem-for-first-order-logic.md), this is equivalence; it is also equivalent to saying that every syntactically consistent first-order theory has a model.

The [compactness theorem](../../../../../../../compactness-theorem.md) states that a set $\Gamma$ of first-order sentences has a model if and only if every finite subset $\Gamma_0\subseteq\Gamma$ has a model. To deduce it, suppose every finite subset is satisfiable but $\Gamma$ is not. Then $\Gamma\models\bot$, so completeness gives a formal proof $\Gamma\vdash\bot$. A proof uses only finitely many assumptions, yielding some finite $\Gamma_0\vdash\bot$, contrary to that subset's satisfiability.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [16H](../../../16h.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
