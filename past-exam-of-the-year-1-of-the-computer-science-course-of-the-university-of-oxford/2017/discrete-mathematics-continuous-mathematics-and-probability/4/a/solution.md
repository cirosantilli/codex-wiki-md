<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [gradient](../../../../../gradient.md) equations are

$$
f_x=3x^2+2xy-10x-9=0,\qquad f_y=x^2-9=0.
$$

Thus $x=3$ gives $y=2$, while $x=-3$ gives $y=8$. The [Hessian matrix](../../../../../hessian-matrix.md) is

$$
H=\begin{pmatrix}6x+2y-10&2x\\2x&0\end{pmatrix},\qquad\det H=-4x^2.
$$

At both critical points the determinant is $-36<0$, so the Hessian is indefinite and the [second-derivative test](../../../../../second-derivative-test.md) classifies both as [saddle points](../../../../../saddle-point.md). Direct substitution gives

$$
\boxed{(3,2),\ (-3,8)\text{ are saddle points, and }f(3,2)=f(-3,8)=-30.}
$$

The factorization $f+30=(x^2-9)(x+y-5)$ also shows the crossing level-set branches through each saddle.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
