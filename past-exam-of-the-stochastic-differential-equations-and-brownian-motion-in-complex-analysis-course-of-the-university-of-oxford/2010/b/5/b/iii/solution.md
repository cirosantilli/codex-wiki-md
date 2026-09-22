<h1 id="b/5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\rho=|z|$. The [triangle inequality](../../../../../../triangle-inequality.md) gives $1-\rho\leq|z-e^{i\theta}|\leq1+\rho$, so the [Poisson kernel for the unit disk](../../../../../../poisson-kernel-for-the-unit-disk.md) obeys

$$
\frac{1-\rho}{1+\rho}\leq
\frac{1-|z|^2}{|z-e^{i\theta}|^2}
\leq\frac{1+\rho}{1-\rho}.
$$

If $\rho\leq r$, replace the lower bound by $(1-r)/(1+r)$ and the upper bound by $(1+r)/(1-r)$. Integrating against the positive measure $h(e^{i\theta})d\theta/(2\pi)$ gives

$$
\boxed{\frac{1-r}{1+r}u(0)\leq u(z)\leq\frac{1+r}{1-r}u(0).}
$$

Here $u(0)$ is exactly the uniform boundary average from part (a). Positivity permits multiplication of the pointwise kernel bounds; continuity on the compact circle ensures all integrals are finite. This is the [Harnack inequality on the unit disk](../../../../../../harnack-inequality-on-the-unit-disk.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../split.md)
7. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
