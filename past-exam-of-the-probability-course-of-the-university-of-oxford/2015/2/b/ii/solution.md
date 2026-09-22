<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrating the [joint probability density](../../../../../joint-probability-density.md) across $u<v<2u$ gives the [marginal density](../../../../../marginal-density.md)

$$
f_U(u)=\int_u^{2u}e^{-u}\,dv=u e^{-u},\qquad u>0.
$$

For every $u>0$, the [conditional probability density](../../../../../conditional-density.md) is consequently

$$
f_{V\mid U}(v\mid u)=\frac{f_{U,V}(u,v)}{f_U(u)}
=\frac1u\mathbf1_{\{u<v<2u\}}.
$$

Hence

$$
\boxed{V\mid U=u\sim\operatorname{Unif}(u,2u).}
$$

This also follows from [two independent exponential variables conditioned on their sum](../../../../../two-independent-exponential-variables-conditioned-on-their-sum.md): given $X+Y=u$, the variable $Y$ is uniform on $(0,u)$, and $V=u+Y$. Conditioning on $U=u$ here is defined through the [conditional probability density](../../../../../conditional-density.md), rather than division by $\mathbb P(U=u)$, which is zero. The endpoint $u=0$ lies outside the positive marginal support and needs no specified conditional law.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
