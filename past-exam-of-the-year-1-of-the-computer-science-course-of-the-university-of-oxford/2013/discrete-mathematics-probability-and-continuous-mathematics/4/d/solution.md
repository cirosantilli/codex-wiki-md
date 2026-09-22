<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [critical point](../../../../../critical-point.md) requires $f_x=f_y=0$. Since $y^4+y^2+1>0$ for every real $y$, the first [partial derivative](../../../../../partial-derivative.md) forces $x=0$. The second then reduces to $3y^2-3=0$, so the only [critical points](../../../../../critical-point.md) are $(0,1)$ and $(0,-1)$.

At these points the [Hessian matrix](../../../../../hessian-matrix.md) is diagonal:

$$
H_f(0,1)=\begin{pmatrix}6&0\\0&6\end{pmatrix},\qquad H_f(0,-1)=\begin{pmatrix}6&0\\0&-6\end{pmatrix}.
$$

The first is a [positive-definite matrix](../../../../../positive-definite-matrix.md), giving a strict local minimum; the second is an [indefinite matrix](../../../../../indefinite-matrix.md), giving a [saddle point](../../../../../saddle-point.md). Their values are $f(0,1)=-1$ and $f(0,-1)=3$. Hence

$$
\boxed{(0,1):\text{ strict local minimum, value }-1;\qquad(0,-1):\text{ saddle point, value }3;\qquad\text{no local maxima}.}
$$

The minimum is local: along $x=0$, $f(0,y)=y^3-3y+1$ is unbounded below as $y\to-\infty$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
