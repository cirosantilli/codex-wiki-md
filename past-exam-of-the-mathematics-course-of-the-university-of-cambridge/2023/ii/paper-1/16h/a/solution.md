<h1 id="16h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [compactness theorem](../../../../../../compactness-theorem.md) says that a set $T$ of first-order sentences has a model if and only if every finite subset of $T$ has a model. One direction is immediate: a model of $T$ models every subset. Conversely, suppose every finite subset is satisfiable. If $T$ had no model, then $T\models\bot$. The [Godel completeness theorem](../../../../../../godel-s-completeness-theorem.md) would give a formal proof $T\vdash\bot$. Every proof is finite, so it would use only a finite subset $T_0\subseteq T$, making $T_0$ inconsistent and hence unsatisfiable. This contradiction proves compactness.

The [Upward Lowenheim-Skolem theorem](../../../../../../upward-lowenheim-skolem-theorem.md) says that a first-order theory with an infinite model has models of arbitrarily large cardinality. Fix a cardinal $\kappa$ and expand the language by constants $c_\alpha$ for $\alpha<\kappa$. Add the sentences

$$
c_\alpha\ne c_\beta
\qquad(\alpha\ne\beta)
$$

to $T$. Any finite subset mentions only finitely many new constants, which can be interpreted as distinct elements of the given infinite model. Compactness therefore gives a model of the expanded theory in which the $c_\alpha$ are all distinct. Its reduct is a model of $T$ of cardinality at least $\kappa$. Together with the downward theorem, this gives a model of exactly $\kappa$ whenever $\kappa\geq|L|+\aleph_0$.

The [Downward Lowenheim-Skolem theorem](../../../../../../downward-lowenheim-skolem-theorem.md) says that if $A$ is an infinite $L$-structure and

$$
|L|+\aleph_0\leq\kappa\leq|A|,
$$

then $A$ has an elementary substructure of cardinality $\kappa$. To see why, first choose $\kappa$ elements. For every existential formula, add a Skolem function selecting a witness whenever one exists, and repeatedly close the chosen set under all language operations and these witness functions. There are at most $\kappa$ functions of finite arity, so the closure still has size $\kappa$. Every existential statement true in $A$ with parameters from the closure has a witness in the closure; the Tarski--Vaught test therefore says that the resulting substructure is elementary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16H](../../16h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
