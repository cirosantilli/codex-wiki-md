<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Define the local [mean velocity](../../../../mean-velocity-of-a-kinetic-distribution.md) and [momentum flux](../../../../momentum-flux.md) by

$$
\boxed{\rho\mathbf u=\int\mathbf v f\,d^3v,\qquad
\Pi_{ij}=\int v_iv_j f\,d^3v.}
$$

Here $\rho=\int f\,d^3v$ and $\mathbf u$ is defined where $\rho>0$. The [pressure tensor](../../../../pressure-tensor.md) separates random motion from the bulk [velocity](../../../../velocity.md):

$$
\Pi_{ij}=\rho u_i u_j+P_{ij},\qquad
P_{ij}=\int(v_i-u_i)(v_j-u_j)f\,d^3v.
$$

Integrating the [mean-field alignment equation](../../../../mean-field-alignment-equation.md) over [velocity space](../../../../velocity-space.md) removes the force [divergence](../../../../divergence.md) and gives the [continuity equation](../../../../continuity-equation.md)

$$
\boxed{\partial_t\rho+\nabla_{\mathbf x}\cdot(\rho\mathbf u)=0.}
$$

Its first [velocity moment](../../../../velocity-moment.md) follows by multiplying by $v_i$ and using $\int v_i\partial_{v_j}(fL_j)\,d^3v=-\int fL_i\,d^3v$:

$$
\partial_t(\rho u_i)+\partial_{x_j}\Pi_{ij}=\int fL_i[f]\,d^3v.
$$

Inserting the [mean-field alignment equation](../../../../mean-field-alignment-equation.md)'s force and integrating each particle [velocity](../../../../velocity.md) separately gives

$$
\boxed{\partial_t(\rho\mathbf u)+\nabla_{\mathbf x}\cdot\boldsymbol\Pi
=\int K(\mathbf x,\mathbf x_\star)\bigl[\mathbf u(\mathbf x_\star,t)-\mathbf u(\mathbf x,t)\bigr]\rho(\mathbf x_\star,t)\rho(\mathbf x,t)\,d^3x_\star.}
$$

The right-hand side exchanges [momentum](../../../../momentum-split.md) between positions and aligns their bulk [velocities](../../../../velocity.md). Its spatial [integral](../../../../integral-split.md) vanishes by exchange [symmetry](../../../../symmetry-physics.md), recovering total [momentum conservation](../../../../momentum-conservation.md). No closure for the [pressure tensor](../../../../pressure-tensor.md) is needed for these exact [velocity moment](../../../../velocity-moment.md) identities.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
