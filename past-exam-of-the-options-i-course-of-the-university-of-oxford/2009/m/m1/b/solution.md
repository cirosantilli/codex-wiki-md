<h1 id="m/m1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The inverse transformation is $x=uv$, $y=u(1-v)$, with support $u>0$, $0<v<1$. Its absolute [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\left|\det\begin{pmatrix}v&u\\1-v&-u\end{pmatrix}\right|=u.
$$

The original joint [probability density function](../../../../../probability-density-function.md), by [independence](../../../../../independent-random-variables.md), is $\lambda^2e^{-\lambda(x+y)}$ on the positive quadrant. The [change of variables formula](../../../../../change-of-variables-formula.md) therefore gives

$$
\boxed{f_{U,V}(u,v)=\lambda^2u e^{-\lambda u}\mathbf1_{\{u>0,\ 0<v<1\}}}.
$$

Integrating over $v$ gives

$$
\boxed{f_U(u)=\lambda^2u e^{-\lambda u}\mathbf1_{\{u>0\}}},
$$

the [gamma distribution](../../../../../gamma-distribution.md) of shape two and rate $\lambda$. Integrating over $u$ gives $f_V(v)=1$ on $(0,1)$. The factorization also shows that $U$ and $V$ are independent.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [M1](../../m1.md)
3. [M](../../../m.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
