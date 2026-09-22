<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

Write $p(z)=c\prod_{j=1}^{2m}(z-a_j)$, including root multiplicities. For $|z|>R$ the convergent logarithm series for every factor $1-a_j/z$ defines

$$
L_j(z)=-\sum_{n\ge1}\frac{a_j^n}{n z^n},\qquad e^{L_j}=1-a_j/z.
$$

Choosing either square root of the nonzero leading coefficient gives the [holomorphic square root outside all polynomial roots](../../../../../holomorphic-square-root-outside-all-polynomial-roots.md)

$$
\boxed{h(z)=\sqrt c\,z^m\exp\left(\tfrac12\sum_j L_j(z)\right).}
$$

Its square is $p$. The even degree makes $z^m$ single-valued, avoiding the winding obstruction that an odd degree would create on the exterior annulus.

For the branch behaving as $z^2$ at infinity, the [Laurent series](../../../../../laurent-series.md) is

$$
\sqrt{z^4-z}=z^2(1-z^{-3})^{1/2}
=z^2-\tfrac12z^{-1}-\tfrac18z^{-4}-\cdots.
$$

It converges uniformly on the circle of radius two. Only the coefficient of $z^{-1}$ contributes to its anticlockwise integral, so

$$
\boxed{\int_C\sqrt{z^4-z}\,dz=-\pi i}
$$

for this branch, and $+\pi i$ for the other. These are the two allowed answers.

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
