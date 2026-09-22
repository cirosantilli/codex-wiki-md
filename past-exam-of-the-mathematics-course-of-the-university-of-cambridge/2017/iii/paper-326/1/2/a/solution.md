<h1 id="1/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $M=\mathcal N(K)^\perp$ for a [bounded linear operator](../../../../../../../continuous-linear-operator.md) between [Hilbert spaces](../../../../../../../hilbert-space-split.md). Its restriction $K|_M:M\to\mathcal R(K)$ is bijective. Define the [Moore–Penrose inverse of an operator](../../../../../../../moore-penrose-inverse-of-an-operator.md) by

$$
\boxed{\mathcal D(K^\dagger)=\mathcal R(K)\oplus\mathcal R(K)^\perp,\qquad K^\dagger f=(K|_M)^{-1}P_{\overline{\mathcal R(K)}}f.}
$$

The inverse vanishes on $\mathcal R(K)^\perp$. For each datum in this domain, $K^\dagger f$ is the [minimum-norm least-squares solution](../../../../../../../minimum-norm-least-squares-solution.md); all [least-squares solutions](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) are $K^\dagger f+\mathcal N(K)$. On their natural domains,

$$
K^\dagger K=P_M,\qquad KK^\dagger=P_{\overline{\mathcal R(K)}}.
$$

The equivalent continuity condition is

$$
\boxed{K^\dagger\text{ is continuous in the ambient norms}\iff\mathcal R(K)\text{ is closed}.}
$$

If the range is closed, the inverse restriction is bounded by the [bounded inverse theorem](../../../../../../../bounded-inverse-theorem.md). Conversely, if $\|K^\dagger f\|\leq C\|f\|$ on its domain and $Ku_n$ converges, replace $u_n$ by $P_Mu_n$. The inequality makes these preimages a [Cauchy sequence](../../../../../../../cauchy-sequence.md), whose limit maps to the limiting datum; the range is therefore closed. Boundedness here uses the data [norm](../../../../../../../norm.md), not a graph [norm](../../../../../../../norm.md) that would conceal instability.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
