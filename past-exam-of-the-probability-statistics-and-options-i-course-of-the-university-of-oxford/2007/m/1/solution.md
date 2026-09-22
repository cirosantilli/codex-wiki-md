<h1 id="m/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Uniform area distribution on the unit disk gives

$$
f_{X,Y}(x,y)=\pi^{-1}\mathbf1_{\{x^2+y^2\leq1\}}.
$$

The [Jacobian determinant](../../../../jacobian-determinant.md) has absolute [determinant](../../../../determinant.md) $r$, so

$$
f_{R,\Theta}(r,\theta)=\frac r\pi
\mathbf1_{\{0<r<1,\ 0\leq\theta<2\pi\}}.
$$

Integrating out the other coordinate gives

$$
\boxed{f_R(r)=2r\mathbf1_{(0,1)}(r),\qquad
f_\Theta(\theta)=\frac1{2\pi}\mathbf1_{[0,2\pi)}(\theta).}
$$

The [joint probability density function](../../../../joint-probability-density.md) factors into these two [marginal distribution](../../../../marginal-distribution.md), proving [independence](../../../../independent-random-variables.md) of $R$ and $\Theta$. Finally

$$
\boxed{\mathbb ER=\int_0^1r(2r)dr=\frac23.}
$$

The angle at $R=0$ can be defined arbitrarily, since that event has [probability](../../../../probability.md) zero.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [M](../../m.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
