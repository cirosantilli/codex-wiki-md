<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose a uniform lower bound $\kappa\in\mathbb R$ for the [Hessian matrix](../../../../hessian-matrix.md) of the [confinement potential](../../../../confinement-potential.md), so $D^2V(x)\geq\kappa I$ for every $x$. A sufficient condition is

$$
\boxed{\kappa+\lambda>0,\qquad\widetilde\lambda=\kappa+\lambda.}
$$

Indeed, [convexity](../../../../convex-function.md) of $V(x)-\kappa|x|^2/2$ gives the [confinement energy](../../../../confinement-energy.md) inequality from part (b), now with $\kappa$ possibly negative. Adding it to the equal-mean [interaction energy](../../../../interaction-energy.md) inequality from part (d) gives

$$
\boxed{\mathcal E[\mu_t]\leq(1-t)\mathcal E[\mu]+t\mathcal E[\nu]-\frac{\kappa+\lambda}{2}t(1-t)d_2^2(\mu,\nu).}
$$

This proves positive [displacement convexity](../../../../displacement-convexity.md) on every class with fixed [barycenter](../../../../barycenter.md). In particular, if $D^2V\geq-KI$ with $K\geq0$, the sufficient condition is $\lambda>K$ and one may take $\widetilde\lambda=\lambda-K$. Wherever classical second derivatives exist, the equivalent differential calculation is $\mathcal E''[\mu_t]\geq(\kappa+\lambda)D^2$; the integrated proof also covers the printed growth assumptions.

## ↑ Ancestors (12)

1. [E](../e.md)
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
