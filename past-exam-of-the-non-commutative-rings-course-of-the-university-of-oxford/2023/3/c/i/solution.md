<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [quotient filtration](../../../../../quotient-filtration.md) induced from the [order filtration of a Weyl algebra](../../../../../order-filtration-of-a-weyl-algebra.md). The key step is to identify the entire [associated graded module](../../../../../associated-graded-module.md) of the [left ideal](../../../../../left-ideal.md) $I$, rather than merely take symbols of its displayed generators.

For every member $x^\alpha y^\beta$ of the [ordered monomial basis of a Weyl algebra](../../../../../ordered-monomial-basis-of-a-weyl-algebra.md), right multiplication by the pure $y$-[monomials](../../../../../monomial.md) gives

$$
(x^\alpha y^\beta)y_1^3y_2^2=x^\alpha y^{\beta+(3,2,0,\ldots,0)},\qquad
(x^\alpha y^\beta)y_1^2y_3^3=x^\alpha y^{\beta+(2,0,3,0,\ldots,0)}.
$$

No commuting past an $x_i$ is necessary. It follows that $I$ is exactly the complex [linear span](../../../../../linear-span.md) of the [basis](../../../../../basis.md) [monomials](../../../../../monomial.md) satisfying either

$$
\beta_1\geq3,\ \beta_2\geq2,
\qquad\text{or}\qquad
\beta_1\geq2,\ \beta_3\geq3.
$$

Intersecting this [linear span](../../../../../linear-span.md) with each filtration piece and then taking symbols therefore yields the [monomial ideal](../../../../../monomial-ideal.md)

$$
\operatorname{gr}I=K=(\xi_1^3\xi_2^2,\xi_1^2\xi_3^3)\subseteq A.
$$

By [b](../../b.md),

$$
\operatorname{gr}(R/I)\cong A/K.
$$

To determine its [Krull dimension](../../../../../krull-dimension.md), compute the [radical of an ideal](../../../../../radical-of-an-ideal.md):

$$
\sqrt K=(\xi_1\xi_2,\xi_1\xi_3)
=(\xi_1)\cap(\xi_2,\xi_3).
$$

Indeed, $K$ lies in the displayed intersection, an intersection of [prime ideals](../../../../../prime-ideal.md). Conversely, $(\xi_1\xi_2)^3\in K$ and $(\xi_1\xi_3)^3\in K$, so both generators of that intersection lie in $\sqrt K$. The equality of the intersection with $(\xi_1\xi_2,\xi_1\xi_3)$ follows by factoring out $\xi_1$ and reducing modulo $(\xi_2,\xi_3)$.

The [order characteristic variety of a Weyl algebra module](../../../../../order-characteristic-variety-of-a-weyl-algebra-module.md) in this case has two [irreducible components](../../../../../irreducible-component.md):

$$
V(K)=\{\xi_1=0\}\ \cup\ \{\xi_2=\xi_3=0\}.
$$

They are coordinate [affine spaces](../../../../../affine-space.md) of dimensions $2n-1$ and $2n-2$, respectively, in the $2n$ coordinates $x_1,\ldots,x_n,\xi_1,\ldots,\xi_n$. The [Krull dimension](../../../../../krull-dimension.md) is the larger of these component dimensions. Thus

$$
\boxed{d(R/I)=2n-1.}
$$

In particular, two displayed generators do not force a drop of two in [dimension](../../../../../dimension-vector-space.md): their common factor creates the component $\xi_1=0$ of dimension $2n-1$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the non-commutative rings course of the University of Oxford](../../../../split.md)
6. [Non-commutative rings course of the University of Oxford](../../../../../non-commutative-rings-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
