<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $P(z)=1+z/2+z^2/12$ and $Q(z)=1-z/2+z^2/12$. The zeros of $Q$ are $3\pm i\sqrt3$, so the [stability function](../../../../../../stability-function.md) has no pole in the closed left half-plane. A direct modulus calculation gives

$$
|Q(z)|^2-|P(z)|^2
=-2\operatorname{Re}z\left(1+\frac{|z|^2}{12}\right).
$$

For $\operatorname{Re}z\leq0$ this is nonnegative, and hence $|R(z)|=|P/Q|\leq1$. Therefore **the [Lobatto IIIA method](../../../../../../lobatto-iiia-method.md) is [A-stable](../../../../../../a-stability.md)**. It is not [L-stable](../../../../../../l-stability.md), because $R(z)\to1$ for large negative real $z$; unconditional scalar stability need not strongly damp the stiffest modes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
