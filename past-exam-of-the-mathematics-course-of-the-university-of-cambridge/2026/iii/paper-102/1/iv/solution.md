<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the [Polynomial representation of the Heisenberg Lie algebra](../../../../../../polynomial-representation-of-the-heisenberg-lie-algebra.md) on the infinite-dimensional [polynomial ring](../../../../../../polynomial-ring.md) $\mathbb C[x]$:

$$
a\cdot f=f',
\qquad b\cdot f=xf,
\qquad c\cdot f=f.
$$

The [product rule](../../../../../../product-rule.md) gives $[d/dx,x]=1$, so this is a [Lie algebra representation](../../../../../../lie-algebra-representation.md). It is a [Faithful Lie algebra representation](../../../../../../faithful-lie-algebra-representation.md): if $\alpha(d/dx)+\beta x+\gamma$ is the zero operator, applying it first to $1$ gives $\beta x+\gamma=0$, and then applying the remaining operator to $x$ gives $\alpha=0$.

To prove [irreducibility](../../../../../../irreducible-lie-algebra-representation.md), let $W$ be a nonzero invariant [subspace](../../../../../../vector-subspace.md) and choose a nonzero polynomial in $W$ of least degree. If its degree were positive, repeated [differentiation](../../../../../../derivative.md) would produce a nonzero element of smaller degree, so $W$ contains a nonzero constant. Invariance under multiplication by $x$ then puts every monomial $x^n$ in $W$, and hence $W=\mathbb C[x]$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
