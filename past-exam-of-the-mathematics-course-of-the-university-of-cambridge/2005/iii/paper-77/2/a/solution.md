<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Unscaled Papkovich–Neuber representation](../../../../../../unscaled-papkovich-neuber-representation.md) with $e_k=e^{ikx-ky}$ and harmonic potentials

$$
\boxed{\Phi=(0,iUe_k),\qquad\chi=-\frac{iU}{k}e_k.}
$$

To see how these coefficients arise, start with $\Phi=(0,Ae_k)$ and $\chi=Be_k$. The representation gives

$$
u=ik(Ay+B)e_k,\qquad v=(-A-kB-kAy)e_k.
$$

At $y=0$, the prescribed tangential velocity requires $ikB=U$, while zero normal velocity requires $A=-kB=iU$. Hence the **decaying half-space flow** is

$$
\boxed{u=U(1-ky)e_k,\qquad v=-ikUy e_k,\qquad p=-2i\mu kUe_k.}
$$

The pressure follows from $2\mu\partial_y\Phi_y$. These harmonic potentials verify the [Stokes equation](../../../../../../stokes-equation.md) and [incompressibility](../../../../../../incompressible-flow.md); the polynomial factors do not prevent decay as $y\to\infty$.

For the [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md), $\sigma_{xy}=\mu(u_y+v_x)$ and $\sigma_{yy}=-p+2\mu v_y$. On the boundary $u_y=-2kUe^{ikx}$, $v_x=0$ and $v_y=-ikUe^{ikx}$. Therefore

$$
\boxed{\sigma_{xy}(x,0)=-2\mu kUe^{ikx},\qquad\sigma_{yy}(x,0)=0.}
$$

Take real parts for a physical sinusoidal flow. Together with the normal-velocity result supplied in the question, these formulas give the [Fourier traction map for a viscous half-space](../../../../../../fourier-traction-map-for-a-viscous-half-space.md); for signed wave numbers its resistance coefficient is $2\mu|k|$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
