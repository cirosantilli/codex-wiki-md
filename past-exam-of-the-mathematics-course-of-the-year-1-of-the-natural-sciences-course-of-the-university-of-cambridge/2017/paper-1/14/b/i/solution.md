<h1 id="14/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $G=(x^2+y^2)/2+ax^4/4$, so $f=e^G>0$. Since $f_x=fG_x$ and $f_y=fG_y$, its [stationary points](../../../../../../stationary-point.md) satisfy

$$
y=0,\qquad x(1+ax^2)=0.
$$

The origin occurs for every real $a$. There are two additional points only for $a<0$, at $x=\pm1/\sqrt{-a}$.

At a [stationary point](../../../../../../stationary-point.md), the [Hessian matrix](../../../../../../hessian-matrix.md) simplifies because $\nabla G=0$:

$$
H_f=fH_G=f\begin{pmatrix}1+3ax^2&0\\0&1\end{pmatrix}.
$$

At the origin this is $I$, so **$(0,0)$ is a strict local minimum for every $a$**, with $f=1$. If $a\geq0$ it is also the unique global minimum, since $G\geq0$ with equality only there. For $a<0$, the two extra points have $1+3ax^2=-2$, so their [Hessian](../../../../../../hessian-matrix.md) has opposite-sign [eigenvalues](../../../../../../eigenvalue.md). Thus

$$
\boxed{a<0:\ \left(\pm\frac1{\sqrt{-a}},0\right)\text{ are saddle points},\qquad
f=\exp\!\left(-\frac1{4a}\right).}
$$

There are no [local maxima](../../../../../../local-maximum.md). When $a<0$, the origin is not a global minimum: $f(x,0)\to0$ as $|x|\to\infty$, but $f$ never attains zero.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [14](../../../14.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
