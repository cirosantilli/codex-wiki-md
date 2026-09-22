<h1 id="17c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the method to the [linear test equation](../../../../../../linear-stability-domain.md) $y'=\lambda y$ and put $z=h\lambda$. Solving the implicit stage gives the [stability function](../../../../../../stability-function.md)

$$
\boxed{
R(z)=\frac{1+(1-a)z+\tfrac12(1-2a)z^2}{1-az}}.
$$

If $a\ne1/2$, the quadratic numerator makes $|R(z)|$ unbounded as $z\to-\infty$, so the method cannot be [A-stable](../../../../../../a-stability.md). For $a=1/2$,

$$
R(z)=\frac{1+z/2}{1-z/2},
$$

which is the [trapezoidal rule](../../../../../../trapezoidal-rule.md) stability function and satisfies $|R(z)|\leq1$ whenever $\operatorname{Re}z\leq0$. Therefore

$$
\boxed{\text{the method is A-stable exactly when }a=\frac12}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17C](../../17c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
