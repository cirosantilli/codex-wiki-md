<h1 id="7b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Start from the product of two [Gamma function](../../../../../../gamma-function.md) integrals:

$$
\Gamma(p)\Gamma(q)=
\int_0^\infty\int_0^\infty e^{-(x+y)}x^{p-1}y^{q-1}\,dx\,dy.
$$

Use the [sum-and-ratio substitution for gamma integrals](../../../../../../sum-and-ratio-substitution-for-gamma-integrals.md)

$$
r=x+y,\qquad t=\frac{x}{x+y},\qquad
x=rt,\quad y=r(1-t),
$$

whose Jacobian is $r$. Absolute convergence for $\operatorname{Re}p,\operatorname{Re}q>0$ justifies the change of variables and separates the integral:

$$
\Gamma(p)\Gamma(q)
=\left(\int_0^\infty e^{-r}r^{p+q-1}\,dr\right)
 \left(\int_0^1t^{p-1}(1-t)^{q-1}\,dt\right)
=\Gamma(p+q)B(p,q).
$$

Therefore

$$
\boxed{\ B(p,q)=\frac{\Gamma(p)\Gamma(q)}{\Gamma(p+q)}\ }.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
