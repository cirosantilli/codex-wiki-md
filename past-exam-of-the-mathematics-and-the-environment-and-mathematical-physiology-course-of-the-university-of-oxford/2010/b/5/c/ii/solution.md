<h1 id="b/5/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $X=z/\epsilon$. The travelling equations become $cv_X=f(v)-w+v_{XX}$ and $cw_X=\epsilon(\gamma v-w)$. Hence, for nonzero $O(1)$ speed and $\epsilon\gamma\ll1$, $w$ is constant to leading order across the front.

Writing $p=v_X$ gives the planar system $v_X=p$, $p_X=cp-f(v)+w$. At the outer cubic roots $A=(V_-,0)$ and $B=(V_+,0)$, $f'(V_\pm)<0$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) is $f'(V_\pm)<0$, so both are [saddle points](../../../../../../saddle-point.md). The increasing front is a [heteroclinic orbit](../../../../../../heteroclinic-orbit.md) from the [unstable manifold](../../../../../../unstable-manifold.md) of $A$ to the [stable manifold](../../../../../../stable-manifold.md) of $B$. Varying $c$ supplies the shooting parameter required to match these manifolds. For this cubic one can also construct it explicitly, as in the next solution.

Multiply the second-order equation by $v_X$ and integrate across the front. Because $v_X\to0$ at both ends, the term $\int v_{XX}v_X\,dX=[v_X^2/2]_{-\infty}^\infty$ vanishes. The remaining identity is

$$
\boxed{c(w)=\frac{\displaystyle\int_{V_-(w)}^{V_+(w)}[f(v)-w]\,dv}{\displaystyle\int_{-\infty}^\infty v_X^2\,dX}.}
$$

The denominator is positive for a nonconstant front, so its direction is determined by the signed [area](../../../../../../surface-area.md) between the cubic and the horizontal recovery line: [Maxwell balance for a scalar reaction-diffusion front](../../../../../../maxwell-balance-for-a-scalar-reaction-diffusion-front.md) gives zero speed when that [area](../../../../../../surface-area.md) vanishes.

The [derivative](../../../../../../derivative.md) in the denominator must use the inner coordinate $X$. If one instead uses the source's original $z$ and denotes $J_z=\int v_z^2\,dz$, then $J_z=\epsilon^{-1}\int v_X^2\,dX$ and the identity is $c=\int(f-w)\,dv/(\epsilon J_z)$. Thus the printed $v'(z)$ is valid only if $z$ has silently been reused for the rescaled inner coordinate; with the original coordinate it misses a factor $\epsilon$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../split.md)
7. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
