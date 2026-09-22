<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [critical points](../../../../../critical-point.md) satisfy both first [partial derivatives](../../../../../partial-derivative.md) equal to zero:

$$
h_x=2x+y=0,\qquad h_y=x+3y^2=0.
$$

Substitute $x=-y/2$ into the second equation to get $y(3y-1/2)=0$. Thus the candidates are $(0,0)$ and $(-1/12,1/6)$.

The [Hessian matrix](../../../../../hessian-matrix.md) and its determinant are

$$
H=\begin{pmatrix}2&1\\1&6y\end{pmatrix},\qquad \det H=12y-1.
$$

At $(0,0)$ the determinant is $-1$, so the [Hessian matrix](../../../../../hessian-matrix.md) is indefinite and the point is a **[saddle point](../../../../../saddle-point.md)**. At $(-1/12,1/6)$ the determinant is $1$ and $h_{xx}=2>0$, so the [Hessian matrix](../../../../../hessian-matrix.md) is positive definite and the point is a **strict [local minimum](../../../../../local-minimum.md)**, with value

$$
\boxed{h(-1/12,1/6)=-\frac1{432}}.
$$

There is no local maximum. Along $x=0$, $h(0,y)=y^3$ is unbounded above and below, so there are no global extrema either.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
