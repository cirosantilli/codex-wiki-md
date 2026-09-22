<h1 id="1/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Moore–Penrose inverse of an operator](../../../../../../../moore-penrose-inverse-of-an-operator.md) is the linear map

$$
K^\dagger:\mathcal D(K^\dagger)=\mathcal R(K)\oplus\mathcal R(K)^\perp
\longrightarrow\mathcal N(K)^\perp
$$

that assigns each admissible datum its [minimum-norm least-squares solution](../../../../../../../minimum-norm-least-squares-solution.md). If $f=y+z$ with $y\in\mathcal R(K)$ and $z\in\mathcal R(K)^\perp$, then $K^\dagger f$ is the unique $u\in\mathcal N(K)^\perp$ satisfying $Ku=y$. In particular it vanishes on $\mathcal R(K)^\perp$, and

$$
KK^\dagger f=P_{\overline{\mathcal R(K)}}f,\qquad
K^\dagger Ku=P_{\mathcal N(K)^\perp}u.
$$

The continuity criterion, with the inherited data [norm](../../../../../../../norm.md) on its domain, is

$$
\boxed{K^\dagger\text{ is continuous}\ \Longleftrightarrow\ \mathcal R(K)\text{ is closed}.}
$$

For a closed [operator range](../../../../../../../range-of-a-bounded-linear-operator.md), the restriction of $K$ from $\mathcal N(K)^\perp$ to $\mathcal R(K)$ is a bounded bijection between [Banach spaces](../../../../../../../banach-space-split.md), so its inverse is bounded by the [bounded inverse theorem](../../../../../../../bounded-inverse-theorem.md). Conversely, if $K^\dagger$ is bounded and $Ku_n\to y$, replace each $u_n$ by $P_{\mathcal N(K)^\perp}u_n=K^\dagger Ku_n$. This is a [Cauchy sequence](../../../../../../../cauchy-sequence.md), hence converges to $u$, and $Ku=y$. Thus every limit of range elements remains in the [operator range](../../../../../../../range-of-a-bounded-linear-operator.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
