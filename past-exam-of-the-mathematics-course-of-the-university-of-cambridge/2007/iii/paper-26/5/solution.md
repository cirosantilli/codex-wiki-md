<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $(M_i)_{i\in I}$ be nonempty [first-order structures](../../../../../first-order-structure.md) in one language and let $U$ be an [ultrafilter](../../../../../ultrafilter.md) on $I$. In the [ultraproduct](../../../../../ultraproduct.md) $M=\prod_iM_i/U$, identify functions when $\{i:f(i)=g(i)\}\in U$, interpret functions coordinatewise and relations by their coordinate truth sets. The [Łoś theorem](../../../../../los-theorem.md) states that for every [first-order formula](../../../../../first-order-formula.md) $\varphi$,

$$
\boxed{M\models\varphi([f_1],\ldots,[f_k])\ \Longleftrightarrow\ \{i:M_i\models\varphi(f_1(i),\ldots,f_k(i))\}\in U.}
$$

All interpretations are independent of representatives: changing finitely many arguments on $U$-small sets changes truth only on their finite union, also $U$-small.

Prove the theorem by [structural induction](../../../../../structural-induction.md) on formulas. Terms evaluate coordinatewise by induction on terms. This proves the atomic cases of [logical equality](../../../../../logical-equality.md) and relation symbols. For conjunction, intersect the two truth sets and use the filter laws. For negation, the truth set is complemented, and an [ultrafilter](../../../../../ultrafilter.md) contains exactly one of a set and its complement. These cases supply the other Boolean connectives too.

For the existential step, a witness $[g]$ in the [ultraproduct](../../../../../ultraproduct.md) makes the coordinate truth set for $\psi(g(i),\bar f(i))$ belong to $U$ by the induction hypothesis. That set is contained in the coordinate truth set of $\exists x\,\psi(x,\bar f(i))$, so the latter is in $U$. Conversely, if that existential truth set $J$ belongs to $U$, choose a witness $g(i)$ in $M_i$ for each $i\in J$, and any element of $M_i$ elsewhere. The [axiom of choice](../../../../../axiom-of-choice.md) supplies this function. The induction hypothesis makes $[g]$ a witness in the [ultraproduct](../../../../../ultraproduct.md). Universal quantification follows by negation. This completes the proof.

For the [compactness theorem](../../../../../compactness-theorem.md), take $I$ to be the set of finite subsets of the given theory $T$. For each $s\in I$, choose $M_s\models s$. For $\varphi\in T$, the cone $C_\varphi=\{s:\varphi\in s\}$ is nonempty, and any finite intersection of such cones contains their union as an index. Extend the filter they generate to an [ultrafilter](../../../../../ultrafilter.md) $U$. By the proved [Łoś theorem](../../../../../los-theorem.md), the [ultraproduct](../../../../../ultraproduct.md) satisfies every $\varphi\in T$, because its coordinate truth set contains $C_\varphi\in U$. Thus $\boxed{\prod_{s\in I}M_s/U\models T}$. This proves compactness without assuming it in the ultraproduct construction.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
