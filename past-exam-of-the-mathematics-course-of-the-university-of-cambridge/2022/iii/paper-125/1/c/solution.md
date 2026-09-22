<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Lutz–Nagell theorem](../../../../../../nagell-lutz-theorem.md) says that if

$$
E:y^2=x^3+ax+b,
\qquad a,b\in\mathbb Z,
$$

has nonzero discriminant and $P=(x,y)\in E(\mathbb Q)$ is a torsion point, then $x,y\in\mathbb Z$ and either $y=0$ or

$$
y^2\mid4a^3+27b^2.
$$

For integrality, fix a prime $p$. If a rational point has nonintegral coordinates, its primitive projective coordinates reduce to $O$, so it belongs to the kernel of reduction. The parameter $t=-x/y$ identifies this kernel with the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md) over $p\mathbb Z_p$. The formal logarithm, with the standard separate first-step argument at $p=2$, shows that this group has no nonzero rational torsion. A rational torsion point therefore has nonnegative $p$-adic valuations in both coordinates for every prime $p$, hence integral coordinates.

Suppose now that $y\ne0$. The point $2P$ is again a nonzero torsion point and hence integral. Its $x$-coordinate is $m^2-2x$, where

$$
m=\frac{3x^2+a}{2y}.
$$

Thus $m^2$ is an integer. A rational number whose square is integral is integral, so $2y\mid3x^2+a$ and in particular $y^2\mid(3x^2+a)^2$. The curve equation and the identity

$$
(3x^2+4a)(3x^2+a)^2-27(x^3+ax-b)(x^3+ax+b)=4a^3+27b^2
$$

then prove $y^2\mid4a^3+27b^2$. This is the [divisibility proof in the Nagell–Lutz theorem](../../../../../../divisibility-proof-in-the-nagell-lutz-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
