<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On the unit circle the constraint [gradient](../../../../../gradient.md) $(2x,2y)$ never vanishes. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations are

$$
8x-3y=2\lambda x,\qquad -3x=2\lambda y,\qquad x^2+y^2=1.
$$

A nonzero solution of the first two equations requires

$$
\det\begin{pmatrix}8-2\lambda&-3\\-3&-2\lambda\end{pmatrix}
=4\lambda^2-16\lambda-9=0,
$$

so $\lambda=9/2$ or $\lambda=-1/2$. Multiplying the first equation by $x$, the second by $y$, and adding shows $2f=2\lambda(x^2+y^2)=2\lambda$. Thus each candidate value of $f$ equals its multiplier.

For $\lambda=9/2$, $y=-x/3$, giving $(x,y)=\pm(3,-1)/\sqrt{10}$. For $\lambda=-1/2$, $y=3x$, giving $(x,y)=\pm(1,3)/\sqrt{10}$. Since a continuous function attains its extrema on the [compact set](../../../../../compact-space.md) given by the [unit circle](../../../../../complex-unit-circle.md) and these exhaust the [Lagrange multiplier](../../../../../lagrange-multiplier.md) candidates,

$$
\boxed{f_{\max}=\frac92\text{ at }\pm\frac{(3,-1)}{\sqrt{10}},\qquad
f_{\min}=-\frac12\text{ at }\pm\frac{(1,3)}{\sqrt{10}}.}
$$

Each $\pm$ changes both coordinates together.

## ↑ Ancestors (12)

1. [D](../d.md)
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
