<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [BGK model](../../../../bgk-model.md) from [b](../b.md). Multiply it by $v_i$ and integrate over [velocity space](../../../../velocity-space.md). Matching the [collision invariants](../../../../collision-invariant.md) makes the collision contribution vanish. For the external [force](../../../../force-split.md) term, [integration by parts](../../../../integration-by-parts.md) gives

$$
-\partial_jU\int v_i\partial_{v_j}f\,d^3v=\rho\,\partial_iU.
$$

Define the [momentum flux](../../../../momentum-flux.md) and [force density](../../../../force-density.md) by

$$
\Pi_{ij}=\int v_iv_jf\,d^3v,\qquad F_i=-\rho\,\partial_iU.
$$

The resulting [momentum conservation](../../../../momentum-conservation.md) equation is

$$
\boxed{\partial_t(\rho u_i)+\partial_j\Pi_{ij}=F_i,\qquad \boldsymbol\Pi=\rho\mathbf u\mathbf u+\mathbf P,\qquad \mathbf F=-\rho\nabla U.}
$$

The [pressure tensor](../../../../pressure-tensor.md) is the second central [velocity moment](../../../../velocity-moment.md),

$$
P_{ij}=\int(v_i-u_i)(v_j-u_j)f\,d^3v.
$$

The zeroth [velocity moment](../../../../velocity-moment.md) also supplies the [continuity equation](../../../../continuity-equation.md) $\partial_t\rho+\partial_j(\rho u_j)=0$, which will be needed in [d](../d.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
