<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [gradient](../../../../../gradient.md) vanishes when $4x+3y-1=0$ and $3x+2y-1=0$. Subtracting these equations gives $x+y=0$, so the unique [critical point](../../../../../critical-point.md) is $\boxed{(x,y)=(1,-1)}$, with $f(1,-1)=0$.

The [Hessian matrix](../../../../../hessian-matrix.md) is

$$
H=\begin{pmatrix}4&3\\3&2\end{pmatrix},\qquad \det H=8-9=-1<0.
$$

It is indefinite, so the [critical point](../../../../../critical-point.md) is a **[saddle point](../../../../../saddle-point.md)**. Explicitly, around that point the change is exactly $2u^2+3uv+v^2$: it is positive for $v=0,u\ne0$ and negative for $v=-3u/2,u\ne0$. Thus arbitrarily close points have both larger and smaller values.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
