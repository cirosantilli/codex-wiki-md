<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $m=1$ the conclusion is immediate, so suppose $m\ge2$ and index the terms of an [arithmetic progression](../../../../../arithmetic-progression.md) by $0,\ldots,m-1$. There are only finitely many [equivalence relations](../../../../../equivalence-relation.md) on this index [set](../../../../../set-split.md). Consequently, recording which terms have equal colours produces a [finite colouring](../../../../../finite-coloring.md) of the positive parameter pairs $(a,d)$, even though the original colouring need not be finite.

We use the [Gallai theorem for an integer lattice](../../../../../gallai-theorem-for-an-integer-lattice.md) in this form: a [finite colouring](../../../../../finite-coloring.md) of the positive integer lattice contains a [monochromatic](../../../../../monochromatic-set.md) [homothetic copy](../../../../../homothetic-copy-of-a-finite-configuration.md) of any prescribed finite integer pattern. Patterns with negative coordinates are allowed here by first translating them into the positive quadrant; the translation is absorbed into the base point of the resulting copy.

Consider the finite pattern

$$
F=\bigcup_{0\le r<s<m}\{(su-rv,v-u):0\le u,v<m\}\subseteq\mathbb Z^2.
$$

The [Gallai theorem for an integer lattice](../../../../../gallai-theorem-for-an-integer-lattice.md) supplies integers $a_0,d_0$ and $q>0$ such that every point of $(a_0,d_0)+qF$ lies in the positive quadrant and has the same equality [equivalence relation](../../../../../equivalence-relation.md) $E$. If $E$ has only singleton classes, any parameter pair in this copy gives an [arithmetic progression](../../../../../arithmetic-progression.md) whose colours are pairwise distinct, so the original colouring is [injective](../../../../../injective-function.md) on it.

Otherwise choose $r<s$ with $r\mathrel E s$. For every $u,v\in\{0,\ldots,m-1\}$, the parameter pair

$$
(a,d)=(a_0+q(su-rv),\ d_0+q(v-u))
$$

has relation $E$. Its terms at indices $r$ and $s$ are therefore equally coloured. But these terms simplify to

$$
a+rd=a_0+rd_0+q(s-r)u=:A_u,\qquad
a+sd=a_0+sd_0+q(s-r)v=:B_v.
$$

Thus $c(A_u)=c(B_v)$ for every $u,v$. Fixing $v=0$ proves that all $A_u$ have the same colour. Every $A_u$ is positive, because it is a term of one of the positive-parameter progressions above, and the [common difference](../../../../../common-difference.md) $q(s-r)$ is positive. Hence $(A_u)_{u=0}^{m-1}$ is a [monochromatic](../../../../../monochromatic-set.md) [arithmetic progression](../../../../../arithmetic-progression.md) of length $m$.

The [canonical arithmetic progression dichotomy](../../../../../canonical-arithmetic-progression-dichotomy.md) is therefore **constant or injective on an [arithmetic progression](../../../../../arithmetic-progression.md) of the prescribed length**. The key point is that one equal-colour index pair has been made to vary independently over two complete progressions; a merely [monochromatic](../../../../../monochromatic-set.md) block of parameter pairs would not by itself give this conclusion.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
