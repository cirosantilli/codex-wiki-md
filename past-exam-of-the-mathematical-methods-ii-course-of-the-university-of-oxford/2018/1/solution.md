<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Stokes theorem](../../../stokes-theorem.md) states that for an oriented smooth [surface](../../../topological-surface-split.md) $S$ with compatible oriented boundary $C$ and a continuously differentiable [vector field](../../../vector-field.md),

$$
\oint_C F\cdot d\ell=\int_S(\nabla\times F)\cdot n\,dS.
$$

Here $\nabla\times F=(-2,-2,-2)$, whereas a [normal vector](../../../normal-vector.md) to the specified [plane](../../../plane.md) is $(1,0,-1)$. Their [dot product](../../../dot-product.md) is zero. Thus **every closed curve in that [plane](../../../plane.md) has zero circulation** by the [Stokes theorem](../../../stokes-theorem.md).

The source says “any curve” and displays an ordinary [line integral](../../../line-integral.md), without specifying that it is closed or giving endpoints. An open [curve](../../../curve.md) need not give zero. On the [plane](../../../plane.md), put $z=x-1$ and $dz=dx$; the pulled-back [differential one-form](../../../one-form.md) becomes

$$
F\cdot d\ell=(y-x+1)dx-dy+(x-y)dx=dx-dy=d(x-y).
$$

Therefore the complete endpoint-dependent answer is

$$
\boxed{\int_{P}^{Q}F\cdot d\ell=(x_Q-y_Q)-(x_P-y_P),}
$$

which specializes to zero for a closed [curve](../../../curve.md). For example, the path from $(1,0,0)$ to $(2,0,1)$ lies in the [plane](../../../plane.md) and has integral $1$. This illustrates a [conservative restriction of a vector field to a plane](../../../conservative-restriction-of-a-vector-field-to-a-plane.md) despite nonzero ambient [curl](../../../curl.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2018](../../2018-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
