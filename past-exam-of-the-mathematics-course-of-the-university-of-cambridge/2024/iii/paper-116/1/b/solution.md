<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $U$ witness that $\kappa$ is [measurable](../../../../../../measurable-cardinal.md). Regularity is given, so it remains to prove the [strong limit cardinal](../../../../../../strong-limit-cardinal.md) property. First, every $A\in U$ has cardinality $\kappa$: if $|A|<\kappa$, then

$$
\kappa\setminus A=\bigcap_{\alpha\in A}(\kappa\setminus\{\alpha\})\in U
$$

by nonprincipality and $\kappa$-completeness, contradicting $A\in U$.

Suppose $\lambda<\kappa$ and $2^\lambda\geq\kappa$. Choose an injection $f:\kappa\to\mathcal P(\lambda)$. For each $\xi<\lambda$, exactly one of

$$
A_\xi=\{\alpha<\kappa:\xi\in f(\alpha)\},
\qquad \kappa\setminus A_\xi
$$

lies in $U$. Their chosen intersection lies in $U$ by $\kappa$-completeness. On that intersection every $f(\alpha)$ is the same subset of $\lambda$, contradicting injectivity because every member of $U$ has size $\kappa$. Thus $2^\lambda<\kappa$, and $\kappa$ is strongly inaccessible.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 116](../../../paper-116-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
