<h1 id="a/1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a material [volume](../../../../../../volume.md) moving with the [fluid](../../../../../../fluid.md), the [Reynolds transport theorem](../../../../../../reynolds-transport-theorem.md) gives, componentwise,

$$
\frac d{dt}\int_{V(t)}q\,dV=\int_{V(t)}\bigl(\partial_tq+\nabla\cdot(q\mathbf u)\bigr)\,dV.
$$

For a scalar $q$ this is also $\int_{V(t)}(Dq/Dt+q\nabla\cdot\mathbf u)dV$. Apply the component formula to [momentum](../../../../../../momentum-split.md) [density](../../../../../../density.md) $q=\rho u_i$. Constant [density](../../../../../../density.md) and [incompressibility](../../../../../../incompressible-flow.md) make the integrand $\rho Du_i/Dt$.

The [traction](../../../../../../traction.md) $\mathbf t(\mathbf n)$ is the [force](../../../../../../force-split.md) per unit [area](../../../../../../surface-area.md) exerted by the material outside a surface on the material inside, with outward [unit normal](../../../../../../unit-normal.md) $\mathbf n$. Reversing the normal exchanges the two sides of the same internal surface. Thus $\mathbf t(-\mathbf n)=-\mathbf t(\mathbf n)$ expresses equal and opposite internal contact [forces](../../../../../../force-split.md), the local form of [Newton's third law](../../../../../../newton-s-third-law.md).

With no [body force](../../../../../../body-force.md), [Newton's second law](../../../../../../newton-s-second-law.md) equates the rate of change of the material [volume](../../../../../../volume.md)'s total [momentum](../../../../../../momentum-split.md) to its surface [force](../../../../../../force-split.md). Combining this balance with the transport theorem gives

$$
\boxed{\int_{V(t)}\rho\frac{D\mathbf u}{Dt}\,dV=\int_{\partial V(t)}\mathbf t(\mathbf n)\,dS.}
$$

This is a [vector](../../../../../../vector.md) identity, since the component argument applies to each direction.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../../split.md)
7. [Theoretical mechanics course of the University of Oxford](../../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
