<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $L_0u=(x+1)u''+xu'$. Matching powers in the [regular perturbation](../../../../../regular-perturbation.md) expansion and in the [Taylor series](../../../../../taylor-series.md) of the left endpoint value gives the complete recursive [boundary value problem](../../../../../boundary-value-problem-split.md)

$$
\boxed{L_0y_n=-y_{n-1},\qquad y_n(0)=\frac2{n!},\quad y_n(1)=0,\qquad n\geq1.}
$$

The higher-order left endpoint values are not zero. The [parameter-dependent boundary data in a regular perturbation hierarchy](../../../../../parameter-dependent-boundary-data-in-a-regular-perturbation-hierarchy.md) rule applies here.

First prove uniqueness for any one of these forced problems. The difference $v$ of two solutions obeys $L_0v=0$ and homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md). The positive [integrating factor](../../../../../integrating-factor.md) $r_0=e^x/(x+1)^2$ gives

$$
r_0L_0v=(pv')',\qquad p=\frac{e^x}{x+1}>0.
$$

Multiplication by $\overline v$ and [integration by parts](../../../../../integration-by-parts.md) yield

$$
0=\int_0^1\overline v\,(pv')'\,dx=-\int_0^1p|v'|^2\,dx.
$$

Hence $v'=0$, and the endpoint values force $v=0$. The [kernel](../../../../../kernel-of-a-linear-map-split.md) is trivial: zero is not an [eigenvalue](../../../../../eigenvalue.md) of this homogeneous [Dirichlet boundary value problem](../../../../../dirichlet-problem.md).

Existence is also explicit. For arbitrary smooth forcing $g$ and endpoint values $u(0)=a$, $u(1)=b$, two integrations of $(pu')'=r_0g$ give

$$
u(x)=a+C H(x)+J_g(x),
$$

where

$$
H(x)=\int_0^x(s+1)e^{-s}\,ds=2-(x+2)e^{-x},
\qquad
J_g(x)=\int_0^x(s+1)e^{-s}\int_0^s\frac{e^tg(t)}{(t+1)^2}\,dt\,ds.
$$

Since $H(1)=2-3/e>0$, the unique choice

$$
\boxed{C=\frac{b-a-J_g(1)}{2-3/e}}
$$

always meets the second endpoint value. Starting from the smooth $y_0$, induction with $g=-y_{n-1}$, $a=2/n!$, $b=0$ proves **existence and uniqueness at every order**.

Equivalently, the [Fredholm alternative](../../../../../fredholm-alternative.md) has no compatibility obstruction because the homogeneous [kernel](../../../../../kernel-of-a-linear-map-split.md) vanishes; the corresponding [adjoint operator](../../../../../adjoint-operator.md) has no zero [eigenvalue](../../../../../eigenvalue.md) either. The direct construction above proves this without computing any particular $y_n$ beyond the leading term.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
