<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the reciprocal identity with flow1 the actual body-force-driven flow and flow2 the [rotlet](../../../../../../rotlet.md) auxiliary field. Its [body force](../../../../../../body-force.md) is zero. The large-sphere boundary terms vanish under the usual decay and convergence assumptions for this unbounded body-force problem.

On the [sphere](../../../../../../sphere.md), the actual rigid [velocity](../../../../../../velocity.md) is $\mathbf U+\boldsymbol\Omega\times\mathbf x$. The auxiliary [force](../../../../../../force.md) is zero and its [torque](../../../../../../torque.md) with the outward fluid normal is $\mathbf G$. The actual [torque](../../../../../../torque.md) with that normal is the negative of the [hydrodynamic torque](../../../../../../hydrodynamic-torque.md) on the [sphere](../../../../../../sphere.md), hence zero for a [torque-free](../../../../../../torque-free.md) [sphere](../../../../../../sphere.md). Consequently the surface side of the reciprocal identity is just $\boldsymbol\Omega\cdot\mathbf G$. The volume side is

$$
\int_{r>a}\mathbf u_G\cdot\mathbf f\,dV=\frac{\mathbf G}{8\pi\mu}\cdot\int_{r>a}\frac{\mathbf x\times\mathbf f(\mathbf x)}{r^3}dV.
$$

Since the auxiliary [couple](../../../../../../couple-mechanics.md) is arbitrary,

$$
\boxed{\boldsymbol\Omega=\frac1{8\pi\mu}\int_{r>a}\frac{\mathbf x\times\mathbf f(\mathbf x)}{r^3}dV.}
$$

An unknown translation contributes nothing because the auxiliary [rotlet](../../../../../../rotlet.md) has zero net [force](../../../../../../force.md). This is [body-force-driven rotation of a torque-free sphere](../../../../../../body-force-driven-rotation-of-a-torque-free-sphere.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
