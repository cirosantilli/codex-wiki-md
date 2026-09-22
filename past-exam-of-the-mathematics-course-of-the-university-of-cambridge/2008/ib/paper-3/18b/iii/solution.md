<h1 id="18b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md) are $\partial_t\mathbf v+(\mathbf v\cdot\nabla)\mathbf v=-\nabla p/\rho+\mathbf f$. Here the [vorticity](../../../../../../vorticity.md) is $2\Omega\mathbf e_z$, and direct differentiation gives $(\mathbf v\cdot\nabla)\mathbf v=-\Omega^2(x,y,0)$, whose curl vanishes. Taking the curl therefore gives

$$
2\dot\Omega\mathbf e_z=\nabla\times\mathbf f=(\gamma-\beta)\mathbf e_z,
$$

so

$$
\boxed{\dot\Omega=\frac{\gamma-\beta}{2}.}
$$

For constant force coefficients and the initial rest condition, $\Omega(t)=(\gamma-\beta)t/2$. Only the antisymmetric part of the horizontal force gradient generates rotation; its symmetric part is balanced by pressure.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [18B](../../18b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
