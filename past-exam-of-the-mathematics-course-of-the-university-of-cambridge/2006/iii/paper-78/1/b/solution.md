<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fluid is outside the body, so its normal on the inner boundary is $-n'$. Let $t=\sigma n'$ be [traction](../../../../../../traction.md) on the body's surface from the fluid. For an exterior point and a flow vanishing at infinity, the boundary representation reads

$$
u_i(y)=-\int J_{ij}(y-x)t_j(x)\,dS_x-\int u_j(x)K_{ijk}(y-x)n'_k(x)\,dS_x.
$$

For $r=|y|\gg a$, expand the single layer through its first moment and the double layer through its zeroth moment:

$$
u_i=J_{ij}(y)F_j+\partial_\alpha J_{i\beta}(y)\Sigma_{\alpha\beta}-K_{ijk}(y)U_{jk}+O(r^{-3}),
\qquad \boxed{F=-\int t\,dS.}
$$

The next single-layer and double-layer terms are both $O(r^{-3})$ at fixed body size and boundary data. Differentiating $J$ gives

$$
\partial_\alpha J_{i\beta}=\frac1{8\pi\mu}\left[
\frac{-\delta_{i\beta}y_\alpha+\delta_{i\alpha}y_\beta+\delta_{\alpha\beta}y_i}{r^3}
-\frac{3y_i y_\alpha y_\beta}{r^5}\right].
$$

Hence the dipole terms combine into

$$
\frac1{8\pi\mu}\left[\frac{(\Sigma-\Sigma^T)y+\operatorname{Tr}\Sigma\,y}{r^3}
-\frac{3(y\cdot My)y}{r^5}\right],\qquad M=\Sigma-2\mu U.
$$

The antisymmetric part obeys $(\Sigma-\Sigma^T)y=G\times y$ for $G_j=-\epsilon_{j\alpha\beta}\Sigma_{\alpha\beta}$. For the symmetric trace-free [tensor](../../../../../../tensor.md) $S$, $y\cdot My=y\cdot Sy+(\operatorname{Tr}M)r^2/3$. Also $\operatorname{Tr}\Sigma-\operatorname{Tr}M=2\mu\operatorname{Tr}U=2\mu Q$. Substitution gives

$$
\boxed{u(y)=J(y)F+\frac{G\times y}{8\pi\mu r^3}+\frac{Qy}{4\pi r^3}
-\frac{3(y\cdot Sy)y}{8\pi\mu r^5}+O(r^{-3}).}
$$

This derives the [Stokes far-field multipoles of a deforming body](../../../../../../stokes-far-field-multipoles-of-a-deforming-body.md). **$F$ is the [force](../../../../../../force.md) exerted by the body on the fluid**, the negative of the integrated fluid [traction](../../../../../../traction.md). **$G$ is its [torque](../../../../../../torque.md) on the fluid**: $G=-\int x\times t\,dS$. Their kernels are the [Stokeslet](../../../../../../stokeslet.md) and [rotlet](../../../../../../rotlet.md). **$Q=\int u\cdot n'\,dS$ is the rate of increase of the body's volume**, by the [Reynolds transport theorem](../../../../../../reynolds-transport-theorem.md). It gives a radial source flow with [volume flux](../../../../../../volumetric-flow-rate.md) $Q$. A volume-preserving body has $Q=0$. The trace-free [tensor](../../../../../../tensor.md) $S$ gives the [stresslet](../../../../../../force-dipole-flow.md), which can remain nonzero for a force-free, torque-free swimmer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
