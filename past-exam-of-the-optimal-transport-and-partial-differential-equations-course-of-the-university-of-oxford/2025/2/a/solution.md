<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $D=d_2(\mu,\nu)$ and $z_t(x,y)=(1-t)x+ty$. The [marginal distributions](../../../../marginal-distribution.md) of the optimal [transport plan](../../../../transport-plan.md) $\Pi$ give $\mu_0=\mu$ and $\mu_1=\nu$. Also

$$
\int|z_t|^2\,d\Pi\leq(1-t)\int|x|^2\,d\mu+t\int|y|^2\,d\nu<\infty,
$$

so $\mu_t$ has a finite second [absolute moment](../../../../absolute-moment.md). For $0\leq s<t\leq1$, the [pushforward measure](../../../../pushforward-measure.md) $(z_s,z_t)_\#\Pi$ is a [coupling](../../../../coupling.md) of $\mu_s,\mu_t$. Therefore

$$
d_2(\mu_s,\mu_t)^2\leq\int|z_t-z_s|^2\,d\Pi=(t-s)^2D^2.
$$

Apply the [triangle inequality](../../../../triangle-inequality.md) for the [second Wasserstein distance](../../../../second-wasserstein-distance.md) along $\mu_0,\mu_s,\mu_t,\mu_1$:

$$
D\leq d_2(\mu_0,\mu_s)+d_2(\mu_s,\mu_t)+d_2(\mu_t,\mu_1)\leq sD+(t-s)D+(1-t)D=D.
$$

All inequalities are equalities, including when $D=0$. Thus this [displacement interpolation](../../../../displacement-interpolation.md) is a constant speed [metric geodesic](../../../../metric-geodesic.md):

$$
\boxed{d_2(\mu_s,\mu_t)=|t-s|d_2(\mu,\nu).}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the optimal transport and partial differential equations course of the University of Oxford](../../../split.md)
5. [Optimal transport and partial differential equations course of the University of Oxford](../../../../optimal-transport-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
