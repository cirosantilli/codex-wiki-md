<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The assertion is true.** The standard filtration $\mathbb{CP}^0\subset\cdots\subset\mathbb{CP}^n$ gives one cell in each dimension $0,2,\ldots,2n$. There are no odd-dimensional cells, so all cellular differentials vanish. The [cellular homology theorem](../../../../../../cellular-homology-theorem.md) and the [universal coefficient theorem for cohomology](../../../../../../universal-coefficient-theorem-for-cohomology.md) give one copy of $\mathbb Z$ in each even degree from zero to $2n$, and zero in every other degree.

Let $x$ be the [Poincare dual](../../../../../../poincare-dual.md) of a [projective hyperplane](../../../../../../projective-hyperplane.md), with the complex orientation. It has degree two and evaluates to $+1$ on a [complex projective line](../../../../../../complex-projective-line.md), so it is the positive generator of $H^2$. We use the intersection interpretation of the [cup product](../../../../../../cup-product.md): the product of duals of oriented submanifolds in transverse position is the dual of their oriented intersection. Distinct transverse complex hyperplanes intersect in $\mathbb{CP}^{n-j}$ after $j$ intersections, with positive complex orientation. Thus $x^j$ is the dual of that linear subspace.

Pairing $x^j$ with a transverse linear $\mathbb{CP}^j$ gives one positively oriented intersection point. Therefore $x^j$ is a primitive generator of $H^{2j}$, for every $0\leq j\leq n$. There is no [cohomology](../../../../../../cohomology-split.md) above dimension $2n$, so $x^{n+1}=0$. These facts show that the surjective graded ring map from $\mathbb Z[x]$ has exactly the indicated kernel:

$$
\boxed{H^*(\mathbb{CP}^n;\mathbb Z)\cong\mathbb Z[x]/(x^{n+1}),\qquad |x|=2.}
$$

This proves the [cohomology ring of complex projective space](../../../../../../cohomology-ring-of-complex-projective-space.md), rather than only its additive groups. For $n=0$ it is $\mathbb Z$, with $x=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
