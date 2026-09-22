<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\omega=\log|\Lambda|$, which is smooth because $\Lambda$ is nowhere zero. The [conformal change of the Levi-Civita connection](../../../../../conformal-change-of-the-levi-civita-connection.md) is

$$
\widetilde\Gamma^a{}_{bc}-\Gamma^a{}_{bc}
=C^a{}_{bc}
=\delta^a_b\partial_c\omega+\delta^a_c\partial_b\omega
-g_{bc}g^{ad}\partial_d\omega.
$$

This follows directly by differentiating $\widetilde g_{ab}=e^{2\omega}g_{ab}$ and using $\widetilde g^{ab}=e^{-2\omega}g^{ab}$ in the [Christoffel symbol](../../../../../christoffel-symbol.md) formula.

Let $V=dx/d\tau$ be a [geodesic](../../../../../geodesic.md) tangent for $g$, with $\tau$ an [affine parameter](../../../../../affine-parameter.md). Since $\nabla_VV=0$,

$$
\boxed{
\widetilde\nabla_VV
=2V(\omega)V-g(V,V)\operatorname{grad}_g\omega.
}
$$

For a [null geodesic](../../../../../null-geodesic.md) the second term vanishes. The remaining acceleration is tangent to the same curve and can be removed by changing its parameter. Explicitly set $\widetilde V=fV$, with $f=d\tau/d\widetilde\tau$. Then

$$
\widetilde\nabla_{\widetilde V}\widetilde V
=f^2\left(2\frac{d\omega}{d\tau}+\frac{d\log f}{d\tau}\right)V.
$$

It vanishes when $f=C^{-1}\Lambda^{-2}$, or

$$
\boxed{\frac{d\widetilde\tau}{d\tau}=C\Lambda^2,\qquad C>0.}
$$

This [affine parameter change under conformal rescaling](../../../../../affine-parameter-change-under-conformal-rescaling.md) shows that [conformal preservation of null geodesic paths](../../../../../conformal-preservation-of-null-geodesic-paths.md) means preservation of unparametrized curves; the original [affine parameter](../../../../../affine-parameter.md) usually changes.

For a non-null [geodesic](../../../../../geodesic.md), the component of $\operatorname{grad}_g\omega$ orthogonal to $V$ generally survives. A change of parameter can remove only the tangential component of acceleration. As a concrete example use [Minkowski spacetime](../../../../../minkowski-spacetime.md),

$$
g=-dt^2+dx^2+dy^2+dz^2,\qquad
\Lambda=e^{kx},\quad k\ne0.
$$

The curve $(t,x,y,z)=(\tau,0,0,0)$ is a [timelike geodesic](../../../../../timelike-geodesic.md) for $g$, but along it

$$
\widetilde\nabla_{\partial_t}\partial_t=k\partial_x.
$$

This acceleration is not parallel to $\partial_t$, so the curve is not a [geodesic](../../../../../geodesic.md) of $\widetilde g$ under any reparametrization. Special non-null curves may still be preserved, for example when $\Lambda$ is constant; nullness is the general guarantee.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the general relativity II course of the University of Oxford](../../../../split.md)
6. [General relativity II course of the University of Oxford](../../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
