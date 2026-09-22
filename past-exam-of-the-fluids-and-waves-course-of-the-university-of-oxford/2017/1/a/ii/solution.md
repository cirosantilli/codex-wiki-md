<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $V(t)$ be a smoothly moving material [volume](../../../../../volume.md), carried by a smooth [velocity field](../../../../../velocity-field.md) $\mathbf u$, and let $f$ be continuously differentiable. The material-volume form of the [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md) states

$$
\boxed{\frac d{dt}\int_{V(t)}f\,dV=\int_{V(t)}\left(\frac{Df}{Dt}+f\nabla\cdot\mathbf u\right)dV.}
$$

Equivalently, the [divergence theorem](../../../../../divergence-theorem.md) gives

$$
\frac d{dt}\int_{V(t)}f\,dV=\int_{V(t)}\partial_t f\,dV+\int_{\partial V(t)}f\mathbf u\cdot\mathbf n\,dS,
$$

where $\mathbf n$ is the outward [unit normal vector](../../../../../unit-normal.md). The second integral measures the [flux](../../../../../flux.md) carried across the instantaneous boundary by its motion.

For the proof, use the particle map $\mathbf x=\mathbf X(\mathbf a,t)$ from $V(0)$, with positive [Jacobian determinant](../../../../../jacobian-determinant.md) $J=\det(\partial\mathbf X/\partial\mathbf a)$. [Euler's volume identity](../../../../../euler-s-volume-identity.md) is

$$
\partial_tJ=J\nabla\cdot\mathbf u.
$$

It is the [Jacobian evolution of a smooth flow](../../../../../jacobian-evolution-of-a-smooth-flow.md): if $F=\partial\mathbf X/\partial\mathbf a$, differentiation gives $F_t=(\nabla\mathbf u)F$, and differentiation of the [determinant](../../../../../determinant.md) gives $J_t=J\operatorname{tr}(F^{-1}F_t)=J\nabla\cdot\mathbf u$. The [change of variables](../../../../../change-of-variables-formula.md) formula now moves the integral to the fixed reference [volume](../../../../../volume.md):

$$
\begin{aligned}
\frac d{dt}\int_{V(t)}f\,dV
&=\frac d{dt}\int_{V(0)}f(\mathbf X(\mathbf a,t),t)J\,d\mathbf a\\
&=\int_{V(0)}\left(\frac{Df}{Dt}J+fJ_t\right)d\mathbf a\\
&=\int_{V(t)}\left(\frac{Df}{Dt}+f\nabla\cdot\mathbf u\right)dV.
\end{aligned}
$$

Finally, $Df/Dt+f\nabla\cdot\mathbf u=\partial_t f+\nabla\cdot(f\mathbf u)$, giving the equivalent boundary form.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
