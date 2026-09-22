<h1 id="f/f1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [inverse function theorem](../../../../../inverse-function-theorem.md) states that a $C^1$ map on an open subset of $\mathbb R^2$ has a $C^1$ local inverse near a point where its derivative is invertible; the inverse derivative at the image point is the inverse [matrix](../../../../../matrix.md) of the original derivative.

Put $s=1+x+y$. Quotient differentiation gives

$$
\boxed{Df(x,y)=\frac1{s^2}\begin{pmatrix}1+y&-x\\-y&1+x\end{pmatrix},
\qquad\det Df(x,y)=\frac1{s^3}.}
$$

The entries are smooth and the determinant is nonzero everywhere on the stated domain, so the theorem supplies the required local inverse at every point. The point $(1/3,1/3)$ is the image of $(1,1)$, where

$$
Df(1,1)=\frac19\begin{pmatrix}2&-1\\-1&2\end{pmatrix}.
$$

Consequently

$$
\boxed{Df^{-1}(1/3,1/3)=\begin{pmatrix}6&3\\3&6\end{pmatrix}.}
$$

Directly solving the two rational equations also gives $f^{-1}(u,v)=(u/(1-u-v),v/(1-u-v))$ on $u+v\neq1$, consistent with the derivative calculation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [F1](../../f1.md)
3. [F](../../../f.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
