<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let $s_p$ be the finite stem of a condition $p=(n_p,s_p,A_p)$, and define

$$
f=\bigcup_{p\in G}s_p.
$$

The stems of two conditions in the [generic filter](../../../../../../generic-filter.md) agree on their common domain, because they have a common stronger extension. Hence this union is a function. For every $\ell\in\omega$, the set of conditions with $n_p\geq\ell$ is dense: append values from the nonempty infinite reservoir until the desired length is reached. Genericity therefore makes $f$ total on $\omega$. The generic stems, and thus their union, are available in $M[G]$.

Fix $g\in M\cap\omega^\omega$ and $K\in\omega$. In $M$ form the set

$$
D_{g,K}=\{(n,s,A):\exists k\ (K\leq k<n\ \land\ g(k)<s(k))\}.
$$

We show that it is a [dense subset of a forcing order](../../../../../../dense-subset-of-a-forcing-order.md). Given $p=(n,s,A)$, put $k=\max(n,K)$. Fill the new positions $n,\ldots,k-1$ with any fixed element of $A$, and choose $a\in A$ with $a>g(k)$ for the new position $k$. This is possible because an infinite subset of $\omega$ is unbounded. Let $t$ be the resulting stem of length $k+1$, and keep the reservoir $A$ unchanged. Then

$$
q=(k+1,t,A)\leq p,\qquad q\in D_{g,K}.
$$

Every new stem value came from the old reservoir, exactly as required by the extension relation. The construction is performed in $M$, so $D_{g,K}\in M$ and is internally dense.

Genericity gives a condition in $G\cap D_{g,K}$. Its witnessing coordinate remains fixed in every later stem and hence in $f$, so some $k\geq K$ satisfies $g(k)<f(k)$. Since this holds for every $K$, there are infinitely many such $k$. As $g$ was arbitrary,

$$
\boxed{f\in\omega^\omega\cap M[G],\qquad\forall g\in M\cap\omega^\omega\;\exists^\infty k\;(g(k)<f(k)).}
$$

Thus this [infinite-reservoir stem forcing](../../../../../../infinite-reservoir-stem-forcing.md) produces an [unbounded real over a model](../../../../../../unbounded-real-over-a-model.md), which is precisely the stipulated meaning of bounding $M$.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
