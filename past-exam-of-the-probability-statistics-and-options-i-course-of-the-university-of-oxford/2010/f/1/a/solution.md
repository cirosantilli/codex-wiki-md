<h1 id="f/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [inverse function theorem](../../../../../inverse-function-theorem.md) says that a continuously differentiable map on an open set, with invertible derivative at a point, restricts to a $C^1$ diffeomorphism between neighborhoods of that point and its image. The inverse derivative is the inverse [matrix](../../../../../matrix.md) of the original derivative at the corresponding preimage.

Put $s=1+x+y\ne0$. Differentiating each coordinate gives

$$
\boxed{Df(x,y)=s^{-2}\begin{pmatrix}1+y&-x\\-y&1+x\end{pmatrix},\qquad\det Df=s^{-3}.}
$$

The determinant never vanishes on $\Omega$, so the theorem applies at every point. The image point $(1/3,1/3)$ has preimage $(1,1)$: the equations $x/s=y/s=1/3$ imply $x=y=1$. Therefore

$$
\boxed{Df^{-1}(1/3,1/3)=\left[\frac19\begin{pmatrix}2&-1\\-1&2\end{pmatrix}\right]^{-1}
=\begin{pmatrix}6&3\\3&6\end{pmatrix}.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [F](../../../f.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
