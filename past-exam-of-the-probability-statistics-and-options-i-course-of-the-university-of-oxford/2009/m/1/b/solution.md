<h1 id="m/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [joint density](../../../../../joint-probability-density.md) of $X,Y$ is $\lambda^2e^{-\lambda(x+y)}$ for positive $x,y$. Inverting the transformation gives $x=uv$, $y=u(1-v)$, with absolute [Jacobian determinant](../../../../../jacobian-determinant.md) $u$ and domain $u>0$, $0<v<1$. The [change of variables for probability densities](../../../../../change-of-variables-for-probability-densities.md) gives

$$
\boxed{f_{U,V}(u,v)=\lambda^2u e^{-\lambda u}\mathbf1_{\{u>0,\ 0<v<1\}},\qquad
f_U(u)=\lambda^2u e^{-\lambda u}\mathbf1_{\{u>0\}}.}
$$

The [joint density](../../../../../joint-probability-density.md) factors into the gamma density of $U$ and the uniform density of $V$ on $(0,1)$, so these two transformed variables are independent.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [M](../../../m.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
