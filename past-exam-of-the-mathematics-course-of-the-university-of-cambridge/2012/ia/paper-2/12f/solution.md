<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

For independent [random variables](../../../../../random-variable-split.md), $\{\min(X,Y)>u\}=\{X>u,Y>u\}$ and $\{\max(X,Y)\leq v\}=\{X\leq v,Y\leq v\}$. Factor their [probabilities](../../../../../probability.md) to obtain the [distribution functions of independent minima and maxima](../../../../../distribution-functions-of-independent-minima-and-maxima.md):

$$
\boxed{F_U(u)=1-[1-F_X(u)][1-F_Y(u)],\qquad F_V(v)=F_X(v)F_Y(v)}.
$$

These formulas also allow atoms; no [probability density function](../../../../../probability-density-function.md) assumption is needed.

For independent unit-rate [exponential distributions](../../../../../exponential-distribution.md), $P(U>u)=e^{-2u}$ for $u\geq0$, so $U\sim\operatorname{Exp}(2)$. To establish the [independent minimum and gap of two exponential variables](../../../../../independent-minimum-and-gap-of-two-exponential-variables.md), set $D=V-U$. On either ordering branch, the change of variables is $(X,Y)=(u,u+d)$ or $(u+d,u)$ with unit absolute [Jacobian determinant](../../../../../jacobian-determinant.md). Both contribute $e^{-2u-d}$; ties have [probability](../../../../../probability.md) zero. Thus the [joint probability density](../../../../../joint-probability-density.md) is

$$
f_{U,D}(u,d)=2e^{-2u-d}=(2e^{-2u})(e^{-d}),\qquad u,d>0.
$$

It factors into normalized exponential [probability density functions](../../../../../probability-density-function.md), proving $U\sim\operatorname{Exp}(2)$, $D\sim\operatorname{Exp}(1)$ and their [independence](../../../../../independent-random-variables.md).

The maximum is $V=U+D$. A half-scaled unit-rate exponential has rate two, so the independent pair $(D,U)$ has the same joint law as $(X,Y/2)$. Consequently

$$
\boxed{V\overset d=X+\frac12Y}.
$$

Using the [expected values](../../../../../expected-value.md), [variances](../../../../../variance-split.md) and [independence](../../../../../independent-random-variables.md) of the summands,

$$
\boxed{\mathbb E V=\frac32,\qquad\operatorname{Var}(V)=\frac54}.
$$

The spacing factorization explains why an order statistic can be represented as a sum of independent waiting times.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
