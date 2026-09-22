<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $N(a_1,\ldots,a_m)$ for the limiting [spreading model](../../../../../../spreading-model.md) norm. We show that deleting any one coefficient does not increase it; iteration then gives every finite suppression.

Fix an index $r$, the coefficients, and a small $\eta>0$. Choose a generation threshold so that all the relevant full and shortened combinations beyond it approximate their model norms within $\eta$. Fix the indices before position $r$ beyond this threshold. Since $(x_n)$ is a [weakly null sequence](../../../../../../weakly-null-sequence.md), the [Mazur lemma](../../../../../../mazur-s-lemma.md) gives a finite convex combination

$$
z=\sum_{j\in F}\lambda_jx_j,\qquad\lambda_j\geq0,\quad\sum\lambda_j=1,\quad\|z\|<\eta,
$$

with every $j$ after the fixed prefix. Choose the remaining indices after $\max F$. For every $j\in F$, the full ordered combination with $x_j$ in slot $r$ has norm at most $N(a)+\eta$. Averaging these combinations gives

$$
\left\|\sum_{i\ne r}a_ix_{n_i}+a_rz\right\|\leq N(a)+\eta.
$$

The shortened combination has norm at most $N(a)+(1+|a_r|)\eta$, and approximates its own model norm within $\eta$. Letting $\eta\downarrow0$ proves

$$
\boxed{\left\|\sum_{i\in A}a_ie_i\right\|\leq\left\|\sum_i a_ie_i\right\|}
$$

for every finite set $A$. Thus the model is a [suppression-unconditional basic sequence](../../../../../../suppression-unconditional-basic-sequence.md) with constant one. The convex-combination argument allows the omitted coordinate to sit between two retained coordinates; simply letting a single omitted index tend to infinity with all others fixed would not respect their order.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
