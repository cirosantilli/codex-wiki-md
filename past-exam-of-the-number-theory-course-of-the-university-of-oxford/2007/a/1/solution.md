<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

By [Vieta's formulas](../../../../vieta-s-formulas.md), the elementary [symmetric polynomials](../../../../symmetric-polynomial.md) in the roots give

$$
c_1=-(\alpha_1+\alpha_2+\alpha_3),\qquad
c_2=\alpha_1\alpha_2+\alpha_2\alpha_3+\alpha_3\alpha_1,\qquad
c_3=-\alpha_1\alpha_2\alpha_3.
$$

For each root, $\alpha_j^3+c_1\alpha_j^2+c_2\alpha_j+c_3=0$. Multiplying by $\alpha_j^k$ and summing gives the [power sum](../../../../power-sum-symmetric-polynomial.md) recurrence

$$
\boxed{s_{k+3}+c_1s_{k+2}+c_2s_{k+1}+c_3s_k=0\qquad(k\ge0).}
$$

Its initial values are $s_0=3$, $s_1=-c_1$ and $s_2=c_1^2-2c_2$. They are [polynomials](../../../../polynomial-split.md) with [integer](../../../../integer-split.md) coefficients in $c_1,c_2,c_3$. The recurrence uses only addition and multiplication by those coefficients, so [induction](../../../../mathematical-induction.md) proves the same for every $s_k$. This is the cubic case of [Newton's identities](../../../../newton-s-identities.md).

For $c_1=0$, put $\alpha_1=u$, $\alpha_2=v$, $\alpha_3=-u-v$. Then $c_2=-(u^2+uv+v^2)$ and $c_3=uv(u+v)$. Expanding the product of root differences gives

$$
\begin{aligned}
\Delta&=(u-v)^2(u+2v)^2(2u+v)^2\\
&=4(u^2+uv+v^2)^3-27u^2v^2(u+v)^2
=\boxed{-4c_2^3-27c_3^2}.
\end{aligned}
$$

This is the [discriminant of a depressed cubic](../../../../discriminant-of-a-depressed-cubic.md) in depressed form, and the displayed identity also proves its expression in integer-coefficient [symmetric polynomials](../../../../symmetric-polynomial.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
