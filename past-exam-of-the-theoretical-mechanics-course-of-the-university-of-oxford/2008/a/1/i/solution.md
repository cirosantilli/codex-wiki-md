<h1 id="a/1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Label fluid particles by $\mathbf a$, with [flow map](../../../../../flow-map.md) $\mathbf x=\chi(\mathbf a,t)$ satisfying $\chi_t=\mathbf u(\chi,t)$. If $J=\det D_{\mathbf a}\chi$, differentiation of the determinant gives $J_t=J\nabla\cdot\mathbf u$. Pull the material-volume integral back to a fixed initial volume:

$$
\frac d{dt}\int_{V(t)}F\,dV=\frac d{dt}\int_{V(0)}F(\chi(\mathbf a,t),t)J\,d\mathbf a.
$$

The [chain rule](../../../../../chain-rule.md) and the Jacobian identity give the integrand $J(F_t+\mathbf u\cdot\nabla F+F\nabla\cdot\mathbf u)$. Transforming back yields the [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md)

$$
\boxed{\frac d{dt}\int_{V(t)}F\,dV=\int_{V(t)}[F_t+\nabla\cdot(F\mathbf u)]\,dV.}
$$

Equivalently the additional surface [flux](../../../../../flux.md) is $\int_{\partial V(t)}F\mathbf u\cdot\mathbf n\,dS$. The material boundary moves with the same normal [velocity](../../../../../velocity.md) as the fluid, which is the key distinction from a fixed [control volume](../../../../../control-volume.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
