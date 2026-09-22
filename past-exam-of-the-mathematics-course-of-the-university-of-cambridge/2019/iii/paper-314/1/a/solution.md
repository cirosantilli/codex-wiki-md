<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D/Dt=\partial_t+\mathbf u\cdot\nabla$ be the [material derivative](../../../../../../material-derivative.md), and write $h$ for [specific enthalpy](../../../../../../specific-enthalpy.md). The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) and [Gauss's law for magnetism](../../../../../../gauss-s-law-for-magnetism.md) give

$$
\frac{D\mathbf B}{Dt}=(\mathbf B\cdot\nabla)\mathbf u-\mathbf B\nabla\cdot\mathbf u.
$$

Dotting the momentum equation with $\mathbf B$ eliminates the [Lorentz force density](../../../../../../lorentz-force-density.md). Therefore the [cross-helicity](../../../../../../cross-helicity.md) density satisfies

$$
\begin{aligned}
\frac{D(\mathbf u\cdot\mathbf B)}{Dt}
&=-\mathbf B\cdot\nabla\Phi-\frac{\mathbf B\cdot\nabla p}{\rho}
+\mathbf B\cdot\nabla\frac{u^2}{2}-(\mathbf u\cdot\mathbf B)\nabla\cdot\mathbf u.
\end{aligned}
$$

The [first law of thermodynamics](../../../../../../first-law-of-thermodynamics.md) gives $dh=T\,ds+dp/\rho$ for [specific entropy](../../../../../../specific-entropy.md) $s$, without requiring uniform [entropy](../../../../../../entropy.md). Consequently

$$
\partial_t h_c+\nabla\cdot(\mathbf u h_c)
=-\mathbf B\cdot\nabla\left(h+\Phi-\frac{u^2}{2}\right)+T\mathbf B\cdot\nabla s.
$$

Since $\nabla\cdot\mathbf B=0$, the first term on the right is a [divergence](../../../../../../divergence.md). This proves the [cross-helicity conservation law](../../../../../../cross-helicity-conservation-law.md), with flux

$$
\boxed{\mathbf F=\mathbf u(\mathbf u\cdot\mathbf B)+\mathbf B\left(h+\Phi-\frac{u^2}{2}\right).}
$$

For the [perfect gas](../../../../../../ideal-gas.md) used here, $h=\gamma p/[(\gamma-1)\rho]$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
