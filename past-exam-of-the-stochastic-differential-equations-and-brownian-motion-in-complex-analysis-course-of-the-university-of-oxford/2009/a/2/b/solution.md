<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two-dimensional [Itô formula](../../../../../ito-s-lemma.md) gives the local martingale part of $u(X_t,Y_t)$ as $\int_0^t u_x\,dX+\int_0^t u_y\,dY$, with all derivatives evaluated along $(X_s,Y_s)$. Independent Brownian coordinates have brackets $[X]_t=[Y]_t=t$ and $[X,Y]_t=0$. Hence the [quadratic variation](../../../../../quadratic-variation.md) is

$$
\boxed{\langle u(X,Y)\rangle_t
=\int_0^t(u_x^2+u_y^2)(X_s,Y_s)\,ds.}
$$

Similarly, the [quadratic covariation](../../../../../quadratic-covariation.md) with $v(X,Y)$ is

$$
\langle u(X,Y),v(X,Y)\rangle_t
=\int_0^t(u_xv_x+u_yv_y)(X_s,Y_s)\,ds.
$$

Sufficient pointwise conditions are equal gradient lengths and perpendicular gradients:

$$
u_x^2+u_y^2=v_x^2+v_y^2,\qquad u_xv_x+u_yv_y=0.
$$

The [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) $u_x=v_y$, $u_y=-v_x$ imply both. These are the [quadratic covariations of an analytic Brownian image](../../../../../quadratic-covariations-of-an-analytic-brownian-image.md); harmonicity is needed to remove the drift, but the two bracket identities themselves follow just from the displayed derivative relations.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
