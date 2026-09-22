<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md) with $z=h\lambda$, the stage equations give the [stability function](../../../../../../stability-function.md) $R(z)=1+zb^T(I-zA)^{-1}e$. Substitution simplifies it to

$$
R(z)=\frac{1+z/2+z^2/12}{1-z/2+z^2/12}=\frac{N(z)}{D(z)}.
$$

The denominator zeros are $3\pm i\sqrt3$, so no pole lies in the closed left half-plane. Moreover,

$$
|D(z)|^2-|N(z)|^2=-2\operatorname{Re}z\left(1+\frac{|z|^2}{12}\right)\geq0
\quad\text{if }\operatorname{Re}z\leq0.
$$

Thus $|R(z)|\leq1$ throughout that half-plane: **the method is A-stable**. On the imaginary axis its amplification modulus is one. Since $R(z)\to1$ as $z\to-\infty$, it is not [L-stable](../../../../../../l-stability.md); linear stability does not guarantee strong damping of very stiff modes.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [2](../../2.md)
3. [Section I](../../section-i.md)
4. [Paper 69](../../../paper-69-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
