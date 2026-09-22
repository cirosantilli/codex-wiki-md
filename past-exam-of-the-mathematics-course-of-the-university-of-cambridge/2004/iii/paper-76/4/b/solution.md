<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Burgers reduction of weakly nonlinear rightgoing acoustics](../../../../../../burgers-reduction-of-weakly-nonlinear-rightgoing-acoustics.md), with $\theta=t-x$, $X=Mx$, $\partial_t=\partial_\theta$ and $\partial_x=-\partial_\theta+M\partial_X$. The [equation of state](../../../../../../equation-of-state.md) expands as

$$
p=\rho+\frac M2(\gamma-1)\rho^2+O(M^2),\qquad
\rho_1=p_1-\frac{\gamma-1}{2}p_0^2.
$$

At order one, [mass conservation](../../../../../../mass-conservation.md) and [momentum conservation](../../../../../../momentum-conservation.md) give $(\rho_0-u_0)_\theta=0$ and $(u_0-p_0)_\theta=0$. For the pure rightgoing [acoustic wave](../../../../../../acoustic-wave.md) with no independent leading mean density or velocity shift, $\rho_0=u_0=p_0$. This is the background choice implicit in the requested traveling-wave expansion; additional mean components would modify its phase convention. The source's duplicated phrase about expanding $p$ should refer to expanding $\rho$ as well as $u$.

At order $M$, the [mass conservation](../../../../../../mass-conservation.md) equation becomes

$$
(\rho_1-u_1)_\theta+p_{0,X}-(p_0^2)_\theta=0,
$$

whereas the [momentum conservation](../../../../../../momentum-conservation.md) equation becomes

$$
(u_1-p_1)_\theta+p_{0,X}=0.
$$

In the latter equation, the two nonlinear products $\rho_0u_{0,\theta}$ and $-u_0u_{0,\theta}$ cancel. Substitute the [equation of state](../../../../../../equation-of-state.md) relation into the former equation and add the two equations to eliminate the first corrections. The result is

$$
\boxed{p_{0,X}-\frac{\gamma+1}{2}p_0p_{0,\theta}=0}.
$$

The same calculation gives $u_1-p_1=-(\gamma+1)p_0^2/4+C(X)$, so the first corrections may be chosen without an explicit secular factor of $\theta$. This is why the retarded-time description can remain uniform for $|\theta|=O(M^{-1})$, provided the leading profile and its relevant [derivatives](../../../../../../derivative.md) remain bounded over that range and the slow propagation interval.

This [Inviscid Burgers equation](../../../../../../inviscid-burgers-equation.md) can develop a [shock](../../../../../../shock-wave.md), so the source's uniformity assertion needs a pre-shock qualification. If $p_0(\theta,0)=F(\theta)$ and $a=(\gamma+1)/2$, its [method of characteristics](../../../../../../method-of-characteristics.md) gives

$$
p_0=F(s),\qquad \theta=s-aF(s)X,\qquad
p_{0,\theta}=\frac{F'(s)}{1-aXF'(s)}.
$$

The smooth construction ends when this denominator vanishes; if $\max F'>0$, the first such distance is $X_s=[a\max F']^{-1}$.

For viscosity write $\beta=M\nu$ with bounded positive $\nu$. Since $u_{0,xx}=p_{0,\theta\theta}+O(M)$, the order-$M$ [momentum conservation](../../../../../../momentum-conservation.md) equation instead reads $(u_1-p_1)_\theta+p_{0,X}=\nu p_{0,\theta\theta}$. Addition now yields the [viscous Burgers equation](../../../../../../viscous-burgers-equation.md)

$$
\boxed{p_{0,X}-\frac{\gamma+1}{2}p_0p_{0,\theta}
=\frac\nu2p_{0,\theta\theta}=\frac\beta{2M}p_{0,\theta\theta}}.
$$

Its positive [diffusion](../../../../../../diffusion.md) resolves the inviscid steepening rather than supporting an unqualified smooth inviscid expansion through [shock](../../../../../../shock-wave.md) formation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
