# Affine focusing model for the Penrose theorem

↑ **Parent:** [Penrose singularity theorem](penrose-singularity-theorem.md)

The [Null Raychaudhuri equation](null-raychaudhuri-equation.md) is the light-ray version of the [Raychaudhuri equation](friedmann-acceleration-equation.md) associated with [Amal Kumar Raychaudhuri](amal-kumar-raychaudhuri.md). His original work concerned relativistic [cosmology](cosmology-split.md).[research discussion, PDF pp. 4–6, the 1955 paper Relativistic Cosmology](amal-kumar-raychaudhuri-by-jayant-vishnu-narlikar.md) For the normal [null geodesic congruence](null-geodesic-congruence.md) before its first focal point, [null twist](null-twist.md) vanishes. With an [affine parameter](affine-parameter.md) $\lambda$, the four-dimensional equation reduces to the displayed [ordinary differential equation](ordinary-differential-equation.md). The [null shear](null-shear.md) contraction is nonnegative on the transverse [screen space](screen-space-of-a-null-congruence.md), and the [null convergence condition](null-convergence-condition.md) makes the other part of $Q$ nonnegative. Consequently $\theta'\leq-\theta^2/2$.

For $\theta(0)=\theta_0<0$, put $w=-1/\theta>0$. Then

$$
w'=\frac{\theta'}{\theta^2}\leq-\frac12,
\qquad w(\lambda)\leq\frac1{|\theta_0|}-\frac\lambda2.
$$

A regular negative [null expansion](null-expansion.md) therefore cannot persist beyond $\lambda=2/|\theta_0|$ if the [null geodesic](null-geodesic.md) extends that far. The [null focusing theorem](null-focusing-theorem.md) turns this estimate into a focal-point bound. The number refers to an [affine parameter](affine-parameter.md), not the [proper time](proper-time.md) of a light ray, which is zero.

For an original soluble model, prescribe constant $Q$ along one twist-free beam; this does not specify an entire solution of the [Einstein field equations](einstein-field-equations-split.md). Introduce a positive affine scale $L$ and the dimensionless variables

$$
u=\frac\lambda L,\qquad y=L\theta,\qquad q=L^2Q,
\qquad \frac{dy}{du}=-\frac{y^2}{2}-q,\quad y(0)=-2.
$$

For an infinitesimal area $A$ define $a=\sqrt{A/A_0}$ before the first zero. Since $y=2a'/a$, where primes now mean $d/du$, the same model becomes

$$
a''=-\frac q2a,\qquad a(0)=1,\quad a'(0)=-1.
$$

Two independently checkable solutions are

$$
\begin{aligned}
q=0:&\quad a=1-u,\qquad y=-\frac2{1-u},\qquad u_*=1,\\
q=2:&\quad a=\cos u-\sin u,\qquad y=-2\frac{\sin u+\cos u}{\cos u-\sin u},\qquad u_*=\frac\pi4.
\end{aligned}
$$

The nonnegative extra focusing term moves the first zero earlier. Direct substitution into both [ordinary differential equations](ordinary-differential-equation.md) verifies the solutions; numerical integration of the nonlinear equation provides a separate comparison with the linear beam equation.

<a id="image-finite-affine-focusing-in-two-explicitly-defined-raychaudhuri-models"></a>
![](penrose-affine-raychaudhuri-focusing.png)

**[Figure 3](#image-finite-affine-focusing-in-two-explicitly-defined-raychaudhuri-models). Finite affine focusing in two explicitly defined Raychaudhuri models**. Both beams start with $L\theta_0=-2$. Curves show the exact solutions for $q=0$ and $q=2$; circles independently integrate $dy/du=-y^2/2-q$. The first zeros occur at $\lambda=L$ and $\lambda=\pi L/4$, respectively. These are illustrative [ordinary differential equation](ordinary-differential-equation.md) models, not fitted collapse data.

A focal point makes this beam description degenerate, but individual [null geodesics](null-geodesic.md) may continue smoothly through it. Even converging light in [Minkowski spacetime](minkowski-spacetime.md) can form a caustic. Converting local focusing into [null geodesic incompleteness](null-geodesic-incompleteness.md) requires the global step below.

## ↑ Ancestors (6)

1. [Penrose singularity theorem](penrose-singularity-theorem.md)
2. [Null geodesic completeness](null-geodesic-completeness.md)
3. [General relativity](general-relativity-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
