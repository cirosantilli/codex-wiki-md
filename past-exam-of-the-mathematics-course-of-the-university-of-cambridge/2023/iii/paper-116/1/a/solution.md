<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $[f]$ for the equivalence class of $f:\kappa\to V_\lambda$ in the [ultrapower](../../../../../../ultrapower.md)

$$
N=(V_\lambda)^\kappa/U,
$$

and define its membership relation by

$$
[g]\mathrel E[f]
\quad\Longleftrightarrow\quad
\{\xi<\kappa:g(\xi)\in f(\xi)\}\in U.
$$

The [kappa-complete filter](../../../../../../kappa-complete-filter.md) property makes $E$ [well-founded](../../../../../../well-founded-relation.md): an infinite descending $E$-chain would give countably many members of $U$ whose intersection belongs to $U$, and every index in that intersection would yield an infinite descending membership chain, contradicting the [Axiom of foundation](../../../../../../axiom-of-regularity.md). The relation is [extensional](../../../../../../extensional-relation.md) by [Łoś's theorem](../../../../../../los-theorem.md).

The [Mostowski collapse theorem](../../../../../../mostowski-collapse-theorem.md) therefore gives a unique isomorphism $\pi:(N,E)\to(M,\in)$ onto a [transitive set](../../../../../../transitive-set.md) $M$. Recursively, the notation missing from the printed formula may be defined by

$$
\pi([f])=\{\pi([g]):[g]\mathrel E[f]\}.
$$

The value is independent of the representative because it is defined on the ultrapower class $[f]$. Moreover $M\subseteq V_\lambda$: every $f:\kappa\to V_\lambda$ has its range contained in some $V_\alpha$ with $\alpha<\lambda$, since $\kappa<\lambda$ and the [strongly inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md) $\lambda$ is [regular](../../../../../../regular-cardinal.md); induction on the resulting rank bound keeps $\pi([f])$ inside $V_\lambda$.

Define the [ultrapower embedding](../../../../../../ultrapower-embedding.md)

$$
j:V_\lambda\longrightarrow M,
\qquad
j(x)=\pi([\operatorname{const}_x]).
$$

The constant-function map into $N$ is [elementary](../../../../../../elementary-embedding.md) by Łoś's theorem, and $\pi$ is an isomorphism, so their composite $j$ is elementary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 116](../../../paper-116-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
