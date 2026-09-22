<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On a branch with fixed signs of $u,v$ and $uv\ne0$, use $u^2=x+y$ and $v^2=y-x$. Differentiating these identities, or inverting the [Jacobian matrix](../../../../../../jacobian-matrix.md), gives

$$
\boxed{u_x=\frac1{2u},\quad u_y=\frac1{2u},\quad
v_x=-\frac1{2v},\quad v_y=\frac1{2v}.}
$$

The inverse [Jacobian matrix](../../../../../../jacobian-matrix.md) is therefore

$$
\frac{\partial(u,v)}{\partial(x,y)}
=\begin{pmatrix}1/(2u)&1/(2u)\\-1/(2v)&1/(2v)\end{pmatrix}.
$$

These are local [partial derivatives](../../../../../../partial-derivative.md). Choosing the signs specifies an [inverse function](../../../../../../inverse-function.md) on $y>|x|$; the original map has four preimages there and has no single global inverse. At $u=0$ or $v=0$, the displayed inverse derivatives are not finite.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
