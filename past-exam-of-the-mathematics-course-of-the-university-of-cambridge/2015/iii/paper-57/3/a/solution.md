<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $D=\partial_t+w\partial_z$, $w=v_z$, and a prime for $\partial_z$. For the [plane-parallel magnetohydrodynamic flow with imposed shear](../../../../../../plane-parallel-magnetohydrodynamic-flow-with-imposed-shear.md), $\nabla\cdot\mathbf u=w'$, while

$$
(\mathbf u\cdot\nabla)\mathbf u
=w\mathbf v'+a v_x\mathbf e_y,\qquad
(\mathbf B\cdot\nabla)\mathbf u
=B_z\mathbf v'+a B_x\mathbf e_y.
$$

The solenoidal [magnetic field](../../../../../../magnetic-field.md) constraint gives $B_z'=0$. The $z$ component of the [MHD induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) then gives $\partial_tB_z=0$. Thus **$B_z$ is constant in both space and time**.

Use the [magnetic tension](../../../../../../magnetic-tension.md) and [magnetic pressure](../../../../../../magnetic-pressure.md) decomposition

$$
\mathbf f_L=\frac{B_z}{\mu_0}\mathbf B'
-\left(\frac{B^2}{2\mu_0}\right)'\mathbf e_z.
$$

The [continuity equation](../../../../../../continuity-equation.md) and momentum equation now reduce to

$$
\boxed{\begin{aligned}
D\rho&=-\rho w',\\
Dv_x&=\frac{B_z}{\mu_0\rho}B_x',\\
Dv_y+a v_x&=\frac{B_z}{\mu_0\rho}B_y',\\
Dw&=-g-\frac1\rho\left(p+\frac{B^2}{2\mu_0}\right)'.
\end{aligned}}
$$

The transverse components of the [MHD induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) are

$$
\boxed{DB_x=B_zv_x'-B_xw',\qquad
DB_y=B_zv_y'+aB_x-B_yw'.}
$$

The terms involving $a$ respectively accelerate the flow across the imposed [shear flow](../../../../../../shear-flow.md) and wind the transverse [magnetic field](../../../../../../magnetic-field.md). The closure is the [isothermal equation of state](../../../../../../globally-isothermal-equation-of-state.md) $p=c_s^2\rho$, as printed in the PDF.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
