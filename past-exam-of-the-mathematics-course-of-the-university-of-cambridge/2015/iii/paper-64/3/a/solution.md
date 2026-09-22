<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use perturbations $\mathbf v,\mathbf b,p,\vartheta$ for [velocity](../../../../../../velocity.md), [magnetic field](../../../../../../magnetic-field.md), [magnetohydrodynamic total pressure](../../../../../../magnetohydrodynamic-total-pressure.md) and [buoyancy displacement variable](../../../../../../buoyancy-displacement-variable.md). Set

$$
D_0=\partial_t-\frac32\Omega x\partial_y.
$$

This is advection by the background [Keplerian shearing sheet](../../../../../../keplerian-shearing-sheet.md). Subtracting the equilibrium before retaining first-order terms gives **the nine linearized equations**:

$$
\begin{aligned}
D_0v_x-2\Omega v_y&=-\rho_0^{-1}\partial_xp-N^2\vartheta+\frac{B_0}{4\pi\rho_0}\partial_zb_x,\\
D_0v_y+\frac12\Omega v_x&=-\rho_0^{-1}\partial_yp+\frac{B_0}{4\pi\rho_0}\partial_zb_y,\\
D_0v_z&=-\rho_0^{-1}\partial_zp+\frac{B_0}{4\pi\rho_0}\partial_zb_z,\\
D_0b_x&=B_0\partial_zv_x,\\
D_0b_y&=-\frac32\Omega b_x+B_0\partial_zv_y,\\
D_0b_z&=B_0\partial_zv_z,\\
D_0\vartheta&=v_x,\\
\partial_xv_x+\partial_yv_y+\partial_zv_z&=0,\\
\partial_xb_x+\partial_yb_y+\partial_zb_z&=0.
\end{aligned}
$$

The azimuthal coefficient $\Omega/2$ combines the [Coriolis acceleration](../../../../../../coriolis-acceleration.md) with perturbation advection of the background shear. The $-3\Omega b_x/2$ term is the winding of radial [magnetic field](../../../../../../magnetic-field.md) by that shear. The tidal force cancels when the equations at a fixed position are subtracted; it does not add a separate Eulerian perturbation force. [Magnetic pressure](../../../../../../magnetic-pressure.md) is already included in $p$, leaving only linear [magnetic tension](../../../../../../magnetic-tension.md). In this normalization $\vartheta$ has dimensions of length because $D_0\vartheta=v_x$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
