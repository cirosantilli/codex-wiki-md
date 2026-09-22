<h1 id="13/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Compute the [characteristic polynomial](../../../../../../characteristic-polynomial.md) using $\det(\lambda I-M)$:

$$
\det(\lambda I-M)=\lambda^3-7\lambda^2+6
=(\lambda-1)(\lambda^2-6\lambda-6).
$$

Its three distinct real roots are $1$ and $3\pm\sqrt{15}$. For $\lambda=1$, the first row of $(M-I)v=0$ gives $z=3y$ and the second then gives $x=y$, so take $v_1=(1,1,3)^T$.

For either root of $\lambda^2-6\lambda-6=0$, take $z=1$ and solve the row equations to get $v=(\lambda-8,5-\lambda,1)^T$. Substitution makes the first two row residuals opposite multiples of the quadratic equation and the third zero. Thus a complete choice is

$$
\boxed{\begin{aligned}
\lambda_1&=1,&v_1&=(1,1,3)^T,\\
\lambda_-&=3-\sqrt{15},&v_-&=(-5-\sqrt{15},\ 2+\sqrt{15},\ 1)^T,\\
\lambda_+&=3+\sqrt{15},&v_+&=(-5+\sqrt{15},\ 2-\sqrt{15},\ 1)^T.
\end{aligned}}
$$

Every nonzero [scalar](../../../../../../scalar.md) multiple is another valid [eigenvector](../../../../../../eigenvector.md) in the corresponding one-dimensional [eigenspace](../../../../../../eigenspace.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [13](../../../13.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
