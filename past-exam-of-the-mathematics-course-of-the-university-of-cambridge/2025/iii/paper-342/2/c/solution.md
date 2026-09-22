<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If every $\operatorname{wt}(E_a)<d/2$, then

$$
\operatorname{wt}(E_a^\dagger E_b)
\leq\operatorname{wt}(E_a)+\operatorname{wt}(E_b)<d.
$$

By the definition of the [distance of a stabilizer code](../../../../../../distance-of-a-stabilizer-code.md), no Pauli operator of weight below $d$ is a nontrivial logical operator. Part (b) therefore proves the [local correctability of a stabilizer code](../../../../../../local-correctability-of-a-stabilizer-code.md) for this error set.

The converse fails because pairwise products, rather than individual weights, control correctability. For example, let $P$ be a high-weight Pauli outside $C(\mathcal S)$ and take the error set $\{I,P\}$. If $P$ anticommutes with a stabilizer, then $\Pi P\Pi=0$, while $P^\dagger P=I$; the KL conditions hold even when $\operatorname{wt}(P)\geq d/2$. A still simpler singleton set containing any known unitary Pauli error is always reversible regardless of its weight.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
