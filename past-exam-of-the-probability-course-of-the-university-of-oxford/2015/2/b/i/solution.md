<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The inverse [linear transformation](../../../../../linear-map.md) is

$$
x=2u-v,\qquad y=v-u,
\qquad
\left|\det\frac{\partial(x,y)}{\partial(u,v)}\right|
=\left|\det\begin{pmatrix}2&-1\\-1&1\end{pmatrix}\right|=1.
$$

The positive support $x>0,y>0$ is exactly $u>0$ and $u<v<2u$. The [independence](../../../../../independent-random-variables.md) and rate-one [exponential distributions](../../../../../exponential-distribution.md) give $f_{X,Y}(x,y)=e^{-x-y}$ there. Since $x+y=u$, the [change of variables for probability densities](../../../../../change-of-variables-for-probability-densities.md) yields

$$
\boxed{f_{U,V}(u,v)=e^{-u}\mathbf1_{\{u>0,\ u<v<2u\}}.}
$$

Although the density's value depends only on $u$, its support does not factor as a product of fixed intervals. Thus this expression does not imply [independence](../../../../../independent-random-variables.md) of $U$ and $V$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
