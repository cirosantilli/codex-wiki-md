<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define a natural number to be a [Finite von Neumann ordinal](../../../../../../finite-von-neumann-ordinal.md): an ordinal $n$ such that every nonempty subset of $n$ has a greatest member. This avoids the usual impredicative description of $\mathbb N$ as the intersection of all inductive sets.

Every usual von Neumann natural number

$$
0=\varnothing,
\qquad
n+1=n\cup\{n\}
$$

has this property. The proof is by induction: a nonempty subset of $n+1$ either contains $n$, which is then greatest, or is a nonempty subset of $n$.

Conversely, let $\alpha$ be an ordinal with the stated property. If $\alpha$ were not one of the finite von Neumann ordinals, it would contain every finite ordinal. Indeed, if $n$ were the least finite ordinal not in $\alpha$, ordinal comparability and the presence of all $m<n$ would force $\alpha=n$ or $\alpha=m$ for some $m<n$. The subset

$$
\omega=\{0,1,2,\ldots\}\subseteq\alpha
$$

would then be nonempty and have no greatest element, a contradiction. Thus this definition picks out exactly the natural numbers given by the usual least-inductive-set definition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
