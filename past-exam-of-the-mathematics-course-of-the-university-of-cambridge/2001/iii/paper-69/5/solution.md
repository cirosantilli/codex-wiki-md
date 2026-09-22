<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Interpret $A$ first as an infinitesimal screen area transported along generators of a future [event horizon](../../../../../event-horizon.md), not as the total area of an arbitrary trapped surface. Horizon generators form an affinely parametrized, hypersurface-orthogonal [null geodesic congruence](../../../../../null-geodesic-congruence.md). The two-dimensional screen metric is positive definite. Its optical tensor has zero twist and decomposes as

$$
B_{AB}=\frac12\theta h_{AB}+\widehat\sigma_{AB},\qquad
\theta=\frac{A'}A,\qquad
\sigma^2=\frac12\widehat\sigma_{AB}\widehat\sigma^{AB}\geq0.
$$

The scalar here agrees with the supplied derivative definition: nullness and the affine geodesic equation remove the longitudinal terms in the contracted norm, leaving $B_{AB}B^{AB}-\theta^2/2$.

To derive the focusing equation, vary neighbouring geodesics and let $J$ be their screen Jacobi map. The [geodesic deviation](../../../../../geodesic-deviation.md) equation is $J''=-\mathcal R J$, where $\mathcal R_{AB}=R_{AcBd}p^cp^d$. Hence $B=J'J^{-1}$ satisfies $B'=-B^2-\mathcal R$. Taking its screen trace yields the [Null Raychaudhuri equation](../../../../../null-raychaudhuri-equation.md)

$$
\theta'=-\frac12\theta^2-2\sigma^2-R_{ab}p^ap^b.
$$

Set $a=A^{1/2}$. Since $a'/a=\theta/2$, the [area-square-root optical focusing equation](../../../../../area-square-root-optical-focusing-equation.md) is

$$
\boxed{\frac{a''}a=\frac12\theta'+\frac14\theta^2
=-\frac12R_{ab}p^ap^b-\sigma^2.}
$$

The PDF's plus sign before $\sigma^2$ is inconsistent with its own positive shear definition. This is an actual source error, not an antisymmetrization or curvature-sign convention.

For an explicit check, take a flat-space twist-free beam with screen Jacobi factors $1+\lambda$ and $1-\lambda$, for $|\lambda|<1$. Then

$$
A=1-\lambda^2,\qquad
\sigma^2=(1-\lambda^2)^{-2},\qquad
(A^{1/2})''=-(1-\lambda^2)^{-3/2}.
$$

Its Ricci term is zero, so the result equals $-\sigma^2A^{1/2}$ and has the opposite sign to the printed equation. This is [flat-space anisotropic beam shear focusing](../../../../../flat-space-anisotropic-beam-shear-focusing.md).

Under the [null convergence condition](../../../../../null-convergence-condition.md) $R_{ab}p^ap^b\geq0$, the correct equation gives concavity of each local area square root. Equivalently $\theta'\leq-\theta^2/2$. If a horizon generator had $\theta(\lambda_0)=\theta_0<0$, integration gives a focal point within affine distance at most $2/|\theta_0|$. Such a generator could not remain on an [achronal boundary](../../../../../achronal-boundary.md) beyond the focal point. Under the usual global hypotheses that horizon generators remain regular and future complete, this contradicts their being generators of the [event horizon](../../../../../event-horizon.md). Hence $\theta\geq0$ and $A'=\theta A\geq0$. Integrating over the horizon patches, and including newly joining generators which can add area, proves [Hawking's area theorem](../../../../../hawking-s-area-theorem.md). Global predictability/completeness assumptions are essential; the local differential inequality alone is not a theorem about arbitrary trapped-surface areas.

For the [perfect fluid](../../../../../perfect-fluid.md) stress tensor, null contraction eliminates the pressure-metric term:

$$
T_{ab}p^ap^b=(\rho+p_{\rm fluid})(u_ap^a)^2.
$$

A nonzero null vector cannot be orthogonal to a timelike fluid velocity. Thus the [perfect-fluid null energy condition](../../../../../perfect-fluid-null-energy-condition.md) is precisely

$$
\boxed{\rho+p_{\rm fluid}\geq0.}
$$

Separate requirements $\rho\geq0$ or $p_{\rm fluid}\geq0$ are not needed for this null focusing argument. With the Einstein equation, $R_{ab}p^ap^b=8\pi T_{ab}p^ap^b$.

A [cosmological constant](../../../../../cosmological-constant.md) contributes only a term proportional to $g_{ab}$, whose null contraction is zero:

$$
(G_{ab}+\Lambda g_{ab})p^ap^b=R_{ab}p^ap^b.
$$

Therefore **a nonzero [cosmological constant](../../../../../cosmological-constant.md) does not change the fluid condition or the local area-focusing argument**, though it can change the global asymptotics and which horizons and completeness hypotheses are appropriate.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
