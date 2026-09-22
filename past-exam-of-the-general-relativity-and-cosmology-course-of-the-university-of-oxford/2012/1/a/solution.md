<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\mu=GM/c^2$, $A=1-2\mu/r$ and $B=1+2\mu/r$. For an affinely parametrized [geodesic](../../../../geodesic.md), use the unhalved quadratic [Lagrangian](../../../../lagrangian.md) $\mathcal L=-c^2A\dot t^2+B\dot{\mathbf r}^{,2}$. Its [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are unchanged by this overall normalization. Since $t$ is a cyclic coordinate, $d(-2c^2A\dot t)/d\tau=0$, equivalently

$$
\boxed{\frac d{d\tau}(2c^2A\dot t)=0.}
$$

The spatial derivatives give $\partial\mathcal L/\partial\dot x^i=2B\dot x^i$ and $\partial\mathcal L/\partial x^i=-c^2\dot t^2A_i+\dot{\mathbf r}^{,2}B_i$, where $A_i=\partial_iA$. Therefore

$$
\boxed{\frac d{d\tau}(2B\dot{\mathbf r})+c^2\dot t^2\nabla A-\dot{\mathbf r}^{,2}\nabla B=0.}
$$

For the [connection coefficients](../../../../connection-components.md), take $x^0=ct$, so $g_{00}=-A$ and $g_{ij}=B\delta_{ij}$. Substituting the diagonal [inverse metric](../../../../inverse-metric.md) into the [Christoffel symbol](../../../../christoffel-symbol.md) formula gives all nonzero component types, including lower-index symmetry:

$$
\boxed{\begin{aligned}
\Gamma^0{}_{0i}=\Gamma^0{}_{i0}&=\frac{A_i}{2A}=\frac{\mu x_i}{Ar^3},\\
\Gamma^i{}_{00}&=\frac{A_i}{2B}=\frac{\mu x^i}{Br^3},\\
\Gamma^i{}_{jk}&=\frac{\delta^i_kB_j+\delta^i_jB_k-\delta_{jk}B_i}{2B}
=-\frac{\mu}{Br^3}(\delta^i_kx_j+\delta^i_jx_k-\delta_{jk}x^i).
\end{aligned}}
$$

All other component types vanish. If the time coordinate is $t$ rather than $ct$, replace $\Gamma^i{}_{00}$ by $\Gamma^i{}_{tt}=c^2\Gamma^i{}_{00}$; the displayed time–space mixed coefficients are unchanged. Spatial indices in these formulas are raised with the background Euclidean metric.

For the circular orbit let $u=\mu/R$ and $\Omega=d\phi/dt=\omega/\dot t$. Both $A$ and $B$ are constant along it. The radial spatial equation gives $(1+u)\omega^2=(GM/R^3)\dot t^2$, so, treating the displayed metric coefficients algebraically, $\Omega^2=GM/[R^3(1+u)]$. The [weak-field approximation](../../../../weak-field-approximation.md) securely determines the leading [Keplerian orbit](../../../../kepler-orbit.md) result

$$
\boxed{P_t\simeq2\pi\sqrt{\frac{R^3}{GM}},\qquad P_\tau=\frac{2\pi}{|\omega|},\qquad P_t=\dot t\,P_\tau.}
$$

The time normalization is $-c^2=-c^2A\dot t^2+BR^2\omega^2$, yielding $\dot t=1+3u/2+O(u^2)$ and $P_\tau/P_t=1-3u/2+O(u^2)$. One must distinguish the proper-time angular frequency in the supplied path from the coordinate-time angular frequency. The formal factor $1+u$ in the frequency equation comes from treating the truncated metric as exact; a complete relative post-Newtonian correction to the orbital period would also require the omitted higher-order temporal metric terms.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
