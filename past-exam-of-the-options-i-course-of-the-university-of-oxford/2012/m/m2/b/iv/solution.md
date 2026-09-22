<h1 id="m/m2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $0<x<1$, the conditional density is obtained by dividing the joint density by the positive marginal density:

$$
f_{Y\mid X=x}(y)=\frac{24xy}{12x(1-x)^2}
=\frac{2y}{(1-x)^2},\qquad0\leq y\leq1-x.
$$

Consequently

$$
\boxed{f_{Y\mid X=1/2}(y)=\begin{cases}8y,&0\leq y\leq1/2,\\0,&\text{otherwise},\end{cases}}
$$

which integrates to one. Its [conditional expectation](../../../../../../conditional-expectation.md) is

$$
\boxed{\mathbb E(Y\mid X=1/2)=\int_0^{1/2}y(8y)\,dy=\frac13.}
$$

This uses the usual continuous conditional-density version, defined by the density ratio at a point where $f_X$ is positive; conditioning does not require the event $X=1/2$ itself to have positive [probability](../../../../../../probability.md).

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [M2](../../../m2.md)
4. [M](../../../../m.md)
5. [2012](../../../../../2012-split.md)
6. [Past exam of the options I course of the University of Oxford](../../../../../split.md)
7. [Options I course of the University of Oxford](../../../../../../options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
