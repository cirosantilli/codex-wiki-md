<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The support condition $-y<x<y$ forces $y>0$. As a check, the [joint probability density](../../../../joint-probability-density.md) integrates to

$$
\int_0^\infty\int_{-y}^{y}2e^{-2y}\,dx\,dy=\int_0^\infty4ye^{-2y}\,dy=1.
$$

For any real $x$, the [marginal density](../../../../marginal-density.md) of $X$ is

$$
f_X(x)=\int_{|x|}^\infty2e^{-2y}\,dy=e^{-2|x|}>0.
$$

Dividing the [joint probability density](../../../../joint-probability-density.md) by this [marginal density](../../../../marginal-density.md) gives the [conditional density](../../../../conditional-density.md):

$$
\boxed{f_{Y\mid X=x}(y)=2e^{-2(y-|x|)}\mathbf1_{\{y>|x|\}}.}
$$

Thus, conditionally on $X=x$, $Y-|x|$ has the rate-two [exponential distribution](../../../../exponential-distribution.md).

For $U=X^2$, use the two inverse branches $x=\sqrt u$ and $x=-\sqrt u$. Each branch has absolute [Jacobian determinant](../../../../jacobian-determinant.md) $1/(2\sqrt u)$. Both lie in the original support exactly when $u>0$ and $y>\sqrt u$. The [change of variables for probability densities](../../../../change-of-variables-for-probability-densities.md) therefore yields

$$
\boxed{f_{U,Y}(u,y)=\begin{cases}\displaystyle\frac{2e^{-2y}}{\sqrt u},&u>0,\ y>\sqrt u,\\0,&\text{otherwise}.\end{cases}}
$$

No [atom of a measure](../../../../atom-measure-theory.md) is created at $u=0$, since $\mathbb P(X=0)=0$. The value of the [probability density function](../../../../probability-density-function.md) at this boundary may be assigned arbitrarily. Checking the [integral](../../../../integral-split.md) over $0<u<y^2$ gives $4ye^{-2y}$, which integrates to one.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the probability course of the University of Oxford](../../../split.md)
5. [Probability course of the University of Oxford](../../../../probability-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
