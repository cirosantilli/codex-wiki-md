<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [standard notation for forcing](../../../../../../standard-notation-for-forcing.md): $q\leq p$ means that $q$ is stronger. A [generic filter](../../../../../../generic-filter.md) is nonempty, upward closed and downward directed, and meets every [dense subset of a forcing order](../../../../../../dense-subset-of-a-forcing-order.md) in the ground model. Names below are [forcing names](../../../../../../forcing-name.md) in $M$, with pairs ordered as $(\text{name},\text{condition})$.

The [semantic forcing relation](../../../../../../semantic-forcing-relation.md) is

$$
\boxed{p\Vdash\varphi(\tau_1,\ldots,\tau_n)\ \Longleftrightarrow\ \text{for every }M\text{-generic }K\ni p,\ M[K]\models\varphi(\tau_1^K,\ldots,\tau_n^K).}
$$

Here $\tau^K=\operatorname{val}(\tau,K)$ is the [evaluation of a forcing name](../../../../../../evaluation-of-a-forcing-name.md). Countability of $M$ supplies such [generic filters](../../../../../../generic-filter.md) through every condition by the [Rasiowa–Sikorski lemma](../../../../../../rasiowa-sikorski-lemma.md).

Define the [syntactic forcing relation](../../../../../../syntactic-forcing-relation.md) by mutual well-founded recursion on the [forcing names](../../../../../../forcing-name.md) for the atomic cases, then induction on the [first-order formula](../../../../../../first-order-formula.md). Its membership clause is

$$
p\Vdash^*\sigma\in\tau\ \Longleftrightarrow\ \forall q\leq p\ \exists s\leq q\ \exists(\rho,r)\in\tau\ (s\leq r\ \land\ s\Vdash^*\sigma=\rho).
$$

For equality, first abbreviate

$$
p\Vdash^*\sigma\subseteq\tau\ \Longleftrightarrow\ \forall(\rho,r)\in\sigma\ \forall q\,(q\leq p\land q\leq r\Rightarrow q\Vdash^*\rho\in\tau),
$$

and set $p\Vdash^*\sigma=\tau$ exactly when both inclusions hold. Each recursive call lowers the rank of at least one [forcing name](../../../../../../forcing-name.md) without raising the other. This makes the mutual recursion well-founded.

For a basis of connectives consisting of [logical conjunction](../../../../../../logical-conjunction.md), [negation](../../../../../../negation.md) and existential quantification, the remaining clauses are

$$
\begin{aligned}
p\Vdash^*(\varphi\land\psi)&\Longleftrightarrow(p\Vdash^*\varphi\ \land\ p\Vdash^*\psi),\\
p\Vdash^*\neg\varphi&\Longleftrightarrow\text{no }q\leq p\text{ satisfies }q\Vdash^*\varphi,\\
p\Vdash^*\exists v\,\varphi(v)&\Longleftrightarrow\forall q\leq p\ \exists s\leq q\ \exists\rho\in M^{\mathbb P}\ (s\Vdash^*\varphi(\rho)).
\end{aligned}
$$

The last line is the [existential clause of syntactic forcing](../../../../../../existential-clause-of-syntactic-forcing.md); witnesses need only occur densely, rather than be forced by $p$ itself with one preselected name. Other connectives are defined by logical abbreviations. The recursion gives a definable relation inside $M$ for each fixed [first-order formula](../../../../../../first-order-formula.md), with quantification over the class of its names. If $\mathbb P$ has no greatest element, use [canonical forcing names](../../../../../../canonical-forcing-name.md) $\check a=\{(\check b,p):b\in a,\ p\in\mathbb P\}$, which still evaluate to $a$. It also proves monotonicity: strengthening a condition preserves what it forces. The [forcing theorem](../../../../../../forcing-theorem.md) identifies the two relations and supplies the truth lemma.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
