<h1 id="26i/solution">Solution</h1>

↑ **Parent:** [26I](../26i.md)

A [lambda-system](../../../../../dynkin-system.md) contains the whole space and is closed under complements and countable disjoint unions. Let $\mathcal D$ be the smallest lambda-system containing a [pi-system](../../../../../pi-system.md) $\mathcal P$. For $A\in\mathcal P$, the family of $B\in\mathcal D$ with $A\cap B\in\mathcal D$ is a lambda-system containing $\mathcal P$, hence is all of $\mathcal D$. Fixing $B\in\mathcal D$ and repeating the argument shows $\mathcal D$ is closed under intersections. A lambda-system closed under intersections is a [sigma-algebra](../../../../../sigma-algebra.md), so $\mathcal D=\sigma(\mathcal P)$. This proves the [pi-lambda theorem](../../../../../pi-lambda-theorem.md). If two [probability measures](../../../../../probability-measure.md) agree on $\mathcal P$, the sets on which they agree form a lambda-system; thus they agree on $\sigma(\mathcal P)$.

The nonnegative form of [Fubini's theorem](../../../../../fubini-s-theorem.md), also called [Tonelli theorem](../../../../../tonelli-theorem.md), states that for a nonnegative product-measurable function on two sigma-finite measure spaces, the product integral equals either iterated integral, allowing the value infinity.

For [Lebesgue measure](../../../../../lebesgue-measure.md) on the plane, a bounded interval rectangle $I\times J$ has measure $|I||J|$. Its preimage under $f$ is $(\lambda I)\times(\lambda^{-1}J)$, which has the same measure. Under $g$, its vertical slice at $x\in I$ is $J-sx$, whose one-dimensional Lebesgue measure is $|J|$ by translation invariance. Tonelli therefore gives $\mu(g^{-1}(I\times J))=|I||J|$. Horizontal slices likewise prove the equality for $h$. The interval rectangles form a generating pi-system. Sigma-finite measure uniqueness, obtained by the finite-measure pi-lambda argument on an increasing rectangular exhaustion, extends these equalities to all Borel sets. Completion extends them to all Lebesgue-measurable sets, since Borel null sets and their subsets remain null.

Writing $\lambda^2=c$, matrix multiplication gives

$$
f h g f=\begin{pmatrix}c&-s\\s&c\end{pmatrix}.
$$

Thus rotations through angles in $[0,\pi/2)$ preserve measure. Their inverses and compositions do too; every plane rotation is a finite composition of these, including a right angle as two rotations through $\pi/4$. **Lebesgue measure is invariant under every rotation.**

## ↑ Ancestors (10)

1. [26I](../26i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
