<h1 id="2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The inverse [change of variables](../../../../../change-of-variables-formula.md) is $y_1=uv$, $y_2=(1-u)v$, on $0<u<1$, $v>0$. Its absolute [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\left|\det\begin{pmatrix}v&u\\-v&1-u\end{pmatrix}\right|=v.
$$

The [change of variables for probability densities](../../../../../change-of-variables-for-probability-densities.md) therefore gives

$$
\boxed{f_{U,V}(u,v)=\lambda^2v e^{-\lambda v}\mathbf1_{\{0<u<1,\ v>0\}}.}
$$

This factorizes on a product domain into a unit [uniform density](../../../../../continuous-uniform-distribution.md) in $u$ and a shape-two [Gamma density](../../../../../gamma-density.md) in $v$. Thus **$U$ and $V$ are independent**, with $U\sim\operatorname{Uniform}(0,1)$ and $V\sim\operatorname{Gamma}(2,\lambda)$. This is the shape-$(1,1)$ case of [beta-gamma independence](../../../../../beta-gamma-independence.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
