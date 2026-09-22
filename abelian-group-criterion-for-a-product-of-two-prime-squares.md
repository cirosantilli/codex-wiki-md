# Abelian group criterion for a product of two prime squares

↑ **Parent:** [Sylow theorems](sylow-theorems.md)

Let $p<q$ be distinct [prime numbers](prime-number-split.md). Every [group](group-split.md) of [group order](order-of-a-finite-group.md) $p^2q^2$ is [Abelian](abelian-group.md) if and only if $p$ does not divide $q^2-1$.

For sufficiency, the [Sylow theorems](sylow-theorems.md) make the number of [Sylow p-subgroups](sylow-subgroup.md) one of $1,q,q^2$, congruent to one modulo $p$. The divisibility hypothesis excludes both nontrivial choices, so that subgroup is [normal](normal-distribution.md). The number of [Sylow subgroups](sylow-subgroup.md) for $q$ is one of $1,p,p^2$, congruent to one modulo $q$. The choice $p$ is impossible because $p<q$. If $q$ divided $p^2-1=(p-1)(p+1)$, primality and $q>p$ would force $q=p+1$, hence $(p,q)=(2,3)$; this pair violates the hypothesis. Thus the other [Sylow subgroup](sylow-subgroup.md) is normal too. Their intersection is trivial, and their [group commutators](group-commutator.md) lie in that intersection, so the [group](group-split.md) is their [direct product of groups](direct-product-of-groups.md). A [group](group-split.md) of prime-square order is abelian: its nontrivial [center of a group](center-of-a-group.md) is either the whole group or has cyclic quotient, and a cyclic central quotient also forces commutativity. Both factors are therefore abelian.

For necessity, suppose $p\mid q^2-1$. The [multiplicative group of a finite field is cyclic](multiplicative-group-of-a-finite-field-is-cyclic.md), so $\mathbb F_{q^2}^{\times}$ contains $\alpha$ of order $p$. Let the [cyclic group](cyclic-group.md) $C_{p^2}$ act on the additive [group](group-split.md) of $\mathbb F_{q^2}$ by mapping its generator to multiplication by $\alpha$. This is a well-defined nontrivial [group action](group-action-split.md), since $\alpha^{p^2}=1$. The resulting [semidirect product](semidirect-product.md) has order $p^2q^2$ and is nonabelian, because the generator does not commute with a nonzero field element. Thus a nonabelian [group](group-split.md) of this order exists exactly when $p\mid q^2-1$.

## ↑ Ancestors (7)

1. [Sylow theorems](sylow-theorems.md)
2. [Finite group theory](finite-group-theory-split.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2021/2/c/solution.md)
- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2021/2/d/solution.md)
