<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

The [compactness theorem](../../../../../compactness-theorem.md) for first-order logic says that a set $T$ of first-order sentences has a model if and only if every finite subset of $T$ has a model. The forward implication is immediate. Conversely, if every finite subset is satisfiable, then $T$ is syntactically consistent: any proof of a contradiction would use only finitely many premises. The [Godel completeness theorem](../../../../../godel-s-completeness-theorem.md) then gives a model of $T$.

The [Upward Lowenheim-Skolem theorem](../../../../../upward-lowenheim-skolem-theorem.md) says that a first-order theory with an infinite model has arbitrarily large models. Given an infinite model of $T$ and any cardinal $\kappa$, enlarge the language by constants $c_\alpha$ for $\alpha<\kappa$ and add

$$
c_\alpha\ne c_\beta\qquad(\alpha\ne\beta).
$$

Every finite subset can interpret its finitely many constants as distinct elements of the original infinite model. By the [compactness theorem](../../../../../compactness-theorem.md), the enlarged theory has a model containing at least $\kappa$ distinct elements; its reduct is a model of $T$.

Finally, suppose a set $S$ and a finite set $T$ axiomatize the same class. Let $\tau$ be the conjunction of the sentences in $T$. Since $S\models\tau$, the set $S\cup\{\neg\tau\}$ is unsatisfiable. Compactness gives a finite $S_0\subseteq S$ such that $S_0\models\tau$. Because $\tau\models S$, we also have $S_0\models S$, while $S\models S_0$ is immediate. Therefore **yes: the finite subset $S_0$ axiomatizes the same theory.** This is [finite subaxiomatization from an equivalent finite theory](../../../../../finite-subaxiomatization-from-an-equivalent-finite-theory.md).

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
