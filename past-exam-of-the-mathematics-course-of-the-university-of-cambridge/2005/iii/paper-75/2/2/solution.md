<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Suppress the common [Fourier mode](../../../../../../fourier-mode.md) factor and define the transverse and full [divergences](../../../../../../divergence.md) of the [fluid Lagrangian displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md) by

$$
D_\perp=\frac1r(r\xi_r)'+\frac{im}{r}\xi_\theta,\qquad D=D_\perp+ik\xi_z.
$$

The perturbed [magnetic field](../../../../../../magnetic-field.md) is $\mathbf Q=(\mathbf B_0\cdot\nabla)\boldsymbol\xi-(\boldsymbol\xi\cdot\nabla)\mathbf B_0-\mathbf B_0D$. Its components are

$$
Q_r=ikB_0\xi_r,\qquad Q_\theta=ikB_0\xi_\theta,\qquad Q_z=-B_0D_\perp-B_0'\xi_r.
$$

Thus the magnetic part of the energy integrand is

$$
\frac{|\mathbf Q|^2}{4\pi}=\frac{B_0^2}{4\pi}\left[k^2(|\xi_r|^2+|\xi_\theta|^2)+|D_\perp|^2\right]
+\frac{(B_0')^2}{4\pi}|\xi_r|^2+\frac{B_0B_0'}{4\pi}(D_\perp^*\xi_r+D_\perp\xi_r^*).
$$

Use $p_0'=-B_0B_0'/(4\pi)$ from force balance. The pressure-gradient cross term is

$$
D^*\xi_rp_0'=-\frac{B_0B_0'}{4\pi}D_\perp^*\xi_r+\frac{ikB_0B_0'}{4\pi}\xi_z^*\xi_r.
$$

The current term has the azimuthal cross-product component $\xi_z^*Q_r-\xi_r^*Q_z$, giving

$$
\frac{\mathbf j_0\cdot(\boldsymbol\xi^*\times\mathbf Q)}c=-\frac{ikB_0B_0'}{4\pi}\xi_z^*\xi_r-\frac{B_0B_0'}{4\pi}\xi_r^*D_\perp-\frac{(B_0')^2}{4\pi}|\xi_r|^2.
$$

Every term involving $B_0'$ cancels in the sum, including the possibly complex $\xi_z^*\xi_r$ terms. The [magnetohydrodynamic energy principle](../../../../../../magnetohydrodynamic-energy-principle.md) therefore reduces exactly to

$$
\boxed{\delta W=2\pi L_z\int r\,dr\left[\gamma p_0|D|^2+\frac{B_0^2}{4\pi}\left(|D_\perp|^2+k^2(|\xi_r|^2+|\xi_\theta|^2)\right)\right]\ge0.}
$$

For physical $p_0\ge0$ and positive [adiabatic index](../../../../../../heat-capacity-ratio.md) $\gamma$, every surviving term is nonnegative. On the admissible displacement domain for the supplied functional, squared ideal-mode frequencies cannot be negative. This is the [positive ideal energy of a theta pinch](../../../../../../positive-ideal-energy-of-a-theta-pinch.md), proving absence of exponentially growing ideal modes. The qualification is **stable or marginal, not strictly positive energy for every motion**: at $k=0$, suitable incompressible displacements can have zero energy. As usual, the energy principle presumes regularity and [boundary conditions](../../../../../../boundary-condition.md) eliminating unwanted surface terms; additional external systems are not part of the given functional.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
