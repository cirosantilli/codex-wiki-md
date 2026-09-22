<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work with coefficients $\mathbb F_2$. For $n\ge1$, the [mod-two cohomology ring of real projective space](../../../../../../mod-two-cohomology-ring-of-real-projective-space.md) and the [Künneth theorem](../../../../../../kunneth-theorem.md) give

$$
H^*(\mathbb{RP}^{2n};\mathbb F_2)=\mathbb F_2[z]/(z^{2n+1}),
\qquad
H^*(\mathbb{RP}^{n}\times\mathbb{RP}^{n};\mathbb F_2)
=\mathbb F_2[x,y]/(x^{n+1},y^{n+1}),
$$

where all three generators have degree one. Any [induced map on cohomology](../../../../../../induced-map-on-cohomology.md) has $f^*z=\alpha x+\beta y$, with $\alpha,\beta\in\mathbb F_2$. By naturality of the [cup product](../../../../../../cup-product.md), the only possible term in top degree is

$$
f^*(z^{2n})=(\alpha x+\beta y)^{2n}
=\binom{2n}{n}\alpha^n\beta^n x^ny^n.
$$

All other terms vanish because their exponent of $x$ or $y$ exceeds $n$. But

$$
\binom{2n}{n}=2\binom{2n-1}{n-1}
$$

is even for every $n\ge1$. Thus the displayed top-degree [induced map on cohomology](../../../../../../induced-map-on-cohomology.md) is zero for every $f$.

Both top-degree [homology groups](../../../../../../homology-group.md) are one-dimensional over $\mathbb F_2$, and their dual [cohomology groups](../../../../../../cohomology-group.md) pair with them nondegenerately. Naturality of this evaluation makes $f_*$ dual to $f^*$, so $f_*$ is also zero and cannot be an [isomorphism](../../../../../../isomorphism.md). This is the [mod-two degree obstruction for equal projective factors](../../../../../../mod-two-degree-obstruction-for-equal-projective-factors.md). Consequently

$$
\boxed{\text{There is no such map for any positive }n.}
$$

If zero is included among the allowed values, $\mathbb{RP}^0$ is a point and the unique map is an [isomorphism](../../../../../../isomorphism.md) on $H_0$. In that convention, **the only value is $n=0$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
