<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With $R=0$, substitute $h=X(x)T(t)$ into the dimensional [Boussinesq equation for an unconfined aquifer](../../../../../boussinesq-equation-for-an-unconfined-aquifer.md):

$$
\phi XT'=KT^2(XX')',\qquad
\frac{\phi T'}{KT^2}=\frac{(XX')'}X=-\lambda.
$$

For a positive draining profile, take $\lambda>0$. Normalize $T(t^*)=1$, so $X$ has the dimensions of height. The temporal [ordinary differential equation](../../../../../ordinary-differential-equation.md) integrates to

$$
\boxed{T(t)=\frac1{1+(K\lambda/\phi)(t-t^*)}.}
$$

The spatial [ordinary differential equation](../../../../../ordinary-differential-equation.md) and [boundary conditions](../../../../../boundary-condition.md) are

$$
\boxed{(XX')'+\lambda X=0\quad(0<x<L),\qquad
X(0)=0,\quad X'(L)=0,\quad X>0\text{ on }(0,L].}
$$

Here $\lambda$ has units of inverse length with this normalization. The scale freedom between $X$ and $T$ is fixed by the chosen value $T(t^*)=1$; the amplitude of $X$, and hence $\lambda$, must be matched to the available water.

This [separable aquifer drawdown](../../../../../separable-aquifer-drawdown.md) is exact if the inherited height profile has the separated spatial shape. For a general rainfall-generated [initial condition](../../../../../initial-condition.md), it describes the late drought regime; it cannot reproduce an arbitrary profile at the instant rainfall stops merely by choosing one temporal constant.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
