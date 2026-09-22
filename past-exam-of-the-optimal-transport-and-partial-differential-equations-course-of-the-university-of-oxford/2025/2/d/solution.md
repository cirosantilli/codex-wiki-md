<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define the [barycenter of a measure](../../../../barycenter-of-a-measure-on-a-banach-space.md) by $m_\mu=\int x\,d\mu(x)$. Under $\Pi$, the mean displacement is $\bar q=m_\nu-m_\mu$, and optimality gives $\int|q|^2\,d\Pi=D^2$. Expanding the square under the [product measure](../../../../product-measure.md) yields the [variance identity for independent copies](../../../../variance-identity-for-independent-copies.md):

$$
\frac12\iint|q-q'|^2\,d\Pi\,d\Pi'=\int|q|^2\,d\Pi-\left|\int q\,d\Pi\right|^2=D^2-|m_\nu-m_\mu|^2.
$$

In the classical regime of part (c), the lower bound on the [Hessian matrix](../../../../hessian-matrix.md) of the [interaction potential](../../../../interaction-potential.md) therefore gives

$$
\frac{d^2}{dt^2}\mathcal W[\mu_t]\geq\lambda\left(D^2-|m_\nu-m_\mu|^2\right).
$$

For equal [barycenters](../../../../barycenter.md), this becomes

$$
\boxed{\frac{d^2}{dt^2}\mathcal W[\mu_t]\geq\lambda D^2.}
$$

For the full stated class of [probability measures](../../../../probability-measure.md), prove the [displacement convexity](../../../../displacement-convexity.md) inequality directly. Pointwise strong [convexity](../../../../convex-function.md) of $W$ gives

$$
W((1-t)(x-x')+t(y-y'))\leq(1-t)W(x-x')+tW(y-y')-\frac\lambda2t(1-t)|q-q'|^2.
$$

Integrating, including the $1/2$ in the [interaction energy](../../../../interaction-energy.md), and using the displayed [variance identity for independent copies](../../../../variance-identity-for-independent-copies.md) gives

$$
\mathcal W[\mu_t]\leq(1-t)\mathcal W[\mu]+t\mathcal W[\nu]-\frac\lambda2t(1-t)\left(D^2-|m_\nu-m_\mu|^2\right).
$$

All terms are finite by quadratic growth and finite second [absolute moments](../../../../absolute-moment.md). Equal [barycenters](../../../../barycenter.md) give the claimed $\lambda$-[displacement convexity](../../../../displacement-convexity.md). Also $m_{\mu_t}=(1-t)m_\mu+tm_\nu$, so this [metric geodesic](../../../../metric-geodesic.md) remains in the prescribed fixed-mean class. Applying the same argument to subintervals proves the second derivative bound in the sense of [distributions](../../../../distribution-mathematical-analysis.md) even when a classical derivative has not been justified. The mean restriction is natural: translating all particles together leaves their pairwise differences and hence the [interaction energy](../../../../interaction-energy.md) unchanged.

## ↑ Ancestors (12)

1. [D](../d.md)
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
