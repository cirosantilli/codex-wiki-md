<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We first prove the local algebra fact behind regularity in codimension one. Let $(A,\mathfrak m)$ be a one-dimensional normal Noetherian local domain. Choose $0\ne a\in\mathfrak m$. Its radical is $\mathfrak m$, so some $\mathfrak m^n$ lies in $(a)$; take minimal $n$. If $n=1$, then $\mathfrak m=(a)$. Otherwise choose $b\in\mathfrak m^{n-1}\setminus(a)$ and put $z=b/a$ in the [fraction field](../../../../../../field-of-fractions.md). We have $z\notin A$ but $z\mathfrak m\subseteq A$.

If $z\mathfrak m\subseteq\mathfrak m$, express multiplication by $z$ on a finite generating set of $\mathfrak m$. The [determinant trick](../../../../../../determinant-trick.md) gives a monic polynomial in $z$ annihilating $\mathfrak m$; as this ideal is nonzero in a domain, the polynomial itself vanishes. Normality would then give $z\in A$, a contradiction. Hence there is $u\in\mathfrak m$ with $zu$ a unit of $A$. Every $v\in\mathfrak m$ satisfies $v=u(zv)/(zu)$, proving $\mathfrak m=(u)$. The [maximal ideal](../../../../../../maximal-ideal.md) therefore has one generator in dimension one, so $A$ is a [regular local ring](../../../../../../regular-local-ring.md), indeed a [discrete valuation ring](../../../../../../discrete-valuation-ring.md). This proves [one-dimensional normal local rings are discrete valuation rings](../../../../../../one-dimensional-normal-local-rings-are-discrete-valuation-rings.md) directly.

Now a codimension-one point of the [normal variety](../../../../../../normal-variety.md) has such a [local ring](../../../../../../local-ring.md), and a codimension-zero [local ring](../../../../../../local-ring.md) is a field. Both are regular. Since the algebraically closed ground field is perfect, regularity and smoothness agree for this finite-type variety, and the [Jacobian criterion](../../../../../../jacobian-criterion.md) makes the [singular locus](../../../../../../singular-locus.md) closed. It contains no codimension-zero or codimension-one point. Therefore every [irreducible component](../../../../../../irreducible-component.md) of the [singular locus](../../../../../../singular-locus.md) has codimension at least two, giving

$$
\boxed{\dim\operatorname{Sing}(X)\le d-2.}
$$

For $d\le1$ this means the [singular locus](../../../../../../singular-locus.md) is empty. In particular the singular set itself is the required closed subset, not merely a set contained in some larger one.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
