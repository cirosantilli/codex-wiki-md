<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $\sigma=\omega(\epsilon)t$, $\tau=\epsilon t$, the multiscale [chain rule](../../../../../chain-rule.md) gives $d/dt=(1+\epsilon\Omega_1+\cdots)\partial_\sigma+\epsilon\partial_\tau$. Expanding $F(u_{i,0}+\epsilon u_{i,1})=F(u_{i,0})+\epsilon DF(u_{i,0})u_{i,1}+\cdots$ gives at order one

$$
\boxed{\partial_\sigma u_{i,0}=F(u_{i,0}).}
$$

At order $\epsilon$, moving the linearized reference dynamics to the left gives

$$
\boxed{\widehat Lu_{i,1}=G_i(u_{i,0})+\sum_{j,b}D_{ij}^{ab}(u_{j,0}^b-u_{i,0}^b)-\Omega_1\partial_\sigma u_{i,0}-\partial_\tau u_{i,0},\quad \widehat L=\partial_\sigma-DF(u_{i,0}).}
$$

The component sum runs over the $m$ state variables; the source uses $n$ in its first displayed sum and $m$ later. All functions for the solvability calculation are periodic in $\sigma$ with period one.

Differentiating the autonomous cycle equation $U'=F(U)$ gives $U''=DF(U)U'$, so $U'$ lies in the periodic [null space](../../../../../kernel-of-a-linear-map-split.md) of $\widehat L$. For a [hyperbolic attracting limit cycle](../../../../../hyperbolic-attracting-limit-cycle.md), its tangent direction has [Floquet multiplier](../../../../../floquet-multiplier.md) one and every transverse multiplier has modulus below one. Hence it is the only periodic direction, proving the required one-dimensional [null space](../../../../../kernel-of-a-linear-map-split.md).

Strictly, mere nonlinear stability does not ensure this spectral assertion. In polar coordinates $\dot r=-(r-1)^3$, $\dot\varphi=2\pi$ has an attracting unit-period cycle but neutral radial [linearization](../../../../../linearization.md) at $r=1$, supplying a second periodic solution of the [variational equation](../../../../../variational-equation.md). Thus the intended [phase reduction](../../../../../phase-reduction.md) assumes the usual simple unit [Floquet multiplier](../../../../../floquet-multiplier.md), or equivalently hyperbolic transverse attraction; this assumption is made explicit here.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
