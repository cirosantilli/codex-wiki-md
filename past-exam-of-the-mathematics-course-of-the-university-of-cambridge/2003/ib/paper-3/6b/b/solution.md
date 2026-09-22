<h1 id="6b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At a simple [root of a polynomial](../../../../../../root-of-a-polynomial.md) $x_i$ of $\omega$, differentiating the product gives $\omega'(x_i)=\prod_{k\ne i}(x_i-x_k)\ne0$. Consequently the [Lagrange basis polynomials](../../../../../../lagrange-cardinal-polynomial.md) can be written

$$
\ell_i(x)=\frac{\omega(x)}{(x-x_i)\omega'(x_i)}.
$$

Divide the [polynomial interpolation](../../../../../../polynomial-interpolation.md) identity from part (a) by $\omega(x)$, at points outside the nodes. This gives the [partial fraction decomposition](../../../../../../partial-fraction-decomposition.md)

$$
\boxed{\frac{p(x)}{\omega(x)}=\sum_{i=0}^n\frac{p(x_i)}{\omega'(x_i)}\frac1{x-x_i}.}
$$

Every denominator of $\omega$ is simple, and the [rational function](../../../../../../rational-function.md) is proper because $\deg p<\deg\omega$, so no polynomial part is missing.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6B](../../6b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
