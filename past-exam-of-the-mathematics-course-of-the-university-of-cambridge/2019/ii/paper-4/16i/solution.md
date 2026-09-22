<h1 id="16i/solution">Solution</h1>

↑ **Parent:** [16I](../16i.md)

An [aleph number](../../../../../aleph-number.md) is an infinite [initial ordinal](../../../../../initial-ordinal.md). More explicitly,

$$
\aleph_0=\omega,
\qquad
\aleph_{\alpha+1}=\text{the least cardinal greater than }\aleph_\alpha,
\qquad
\aleph_\lambda=\sup_{\alpha<\lambda}\aleph_\alpha
$$

for a limit ordinal $\lambda$. By the [well-ordering theorem](../../../../../well-ordering-theorem.md), every set is equipotent to an ordinal and hence to a unique initial ordinal. If the set is infinite, that initial ordinal occurs in the aleph enumeration. Thus **every infinite set has cardinality $\aleph_\alpha$ for a unique ordinal $\alpha$**.

We next prove the [square of an infinite cardinal](../../../../../square-of-an-infinite-cardinal.md). Suppose otherwise and let $\kappa$ be the least infinite cardinal for which $\kappa^2>\kappa$. Well-order $\kappa\times\kappa$ by increasing

$$
\max\{\alpha,\beta\},
$$

breaking ties lexicographically. The predecessors of $(\alpha,\beta)$ lie inside $\gamma\times\gamma$ for some $\gamma<\kappa$. If $\mu=|\gamma|$, then $\mu<\kappa$; by minimality, $\mu^2=\mu$ when $\mu$ is infinite, while the finite case is immediate. Every proper initial segment therefore has cardinality less than $\kappa$.

Recursively assign to each pair the least ordinal below $\kappa$ not already assigned to one of its predecessors. Such an ordinal always exists by the preceding bound, so this constructs an injection $\kappa\times\kappa\to\kappa$. The map $\alpha\mapsto(\alpha,0)$ gives the reverse injection, and the [Cantor-Schröder-Bernstein theorem](../../../../../cantor-schroder-bernstein-theorem.md) yields

$$
\boxed{\kappa^2=\kappa.}
$$

For infinite $X_1,\ldots,X_n$, finitely many applications of the [cardinal comparability principle](../../../../../cardinal-comparability-principle.md) let us choose $X_i$ of largest cardinality $\kappa$. Then

$$
\kappa
\leq\left|X_1\cup\cdots\cup X_n\right|
\leq |X_1|+\cdots+|X_n|
\leq n\kappa
=\kappa,
$$

where the final equality follows from infinite cardinal arithmetic. Consequently

$$
\boxed{|X_1\cup\cdots\cup X_n|=|X_i|\text{ for some }i.}
$$

For a countable family of pairwise different infinite cardinalities, the answer is **yes**. Regard initial ordinals as sets and take

$$
X_1=\aleph_\omega,
\qquad
X_{n+2}=\aleph_n\quad(n<\omega).
$$

The cardinalities are pairwise distinct, but every $X_{n+2}$ is a subset of $X_1$. Hence

$$
\boxed{\bigcup_{j\geq1}X_j=X_1,}
$$

which is the [countable family of distinct infinite cardinalities with a largest member](../../../../../countable-family-of-distinct-infinite-cardinalities-with-a-largest-member.md) construction.

## ↑ Ancestors (10)

1. [16I](../16i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
