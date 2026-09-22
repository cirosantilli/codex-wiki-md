<h1 id="38c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Runge-Kutta method](../../../../../../runge-kutta-method.md) has $A=\begin{pmatrix}1/4&1/4-a\\1/4+a&1/4\end{pmatrix}$ and $b=(1/2,1/2)^T$. Solving the stage equations for $y'=\lambda y$ gives the [stability function](../../../../../../stability-function.md)

$$
R(z)=1+z\,b^T(I-zA)^{-1}\mathbf1
=\frac{1+z/2+a^2z^2}{1-z/2+a^2z^2}.
$$

For $a\ne0$, the denominator roots have positive real parts: real roots are positive from their positive sum and product, while a complex conjugate pair has real part $1/(4a^2)>0$. For $a=0$ its sole root is $2$. Thus there are no poles or singular stage systems in the left half-plane.

Writing $z=x+iy$, direct expansion gives

$$
|1-z/2+a^2z^2|^2-|1+z/2+a^2z^2|^2=-2x(1+a^2|z|^2)\ge0\quad(x\le0).
$$

This proves the [A-stability of a symmetric two-stage implicit Runge-Kutta family](../../../../../../a-stability-of-a-symmetric-two-stage-implicit-runge-kutta-family.md):

$$
\boxed{\text{The method is A-stable for every }a\in\mathbb R.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38C](../../38c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
