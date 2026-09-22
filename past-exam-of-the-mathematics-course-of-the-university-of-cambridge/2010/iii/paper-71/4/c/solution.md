<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $\kappa,\omega>0$ and impose upward [group velocity](../../../../../../group-velocity.md) in $z>0$. The two positive-frequency components then have wave vectors $\mathbf k_1=(\kappa,m)$ and $\mathbf k_2=(-\kappa,m)$ with $m<0$. Equal lengths are automatic, and orthogonality gives $m^2=\kappa^2$. Hence

$$
\boxed{m=-\kappa,\qquad \omega=N/\sqrt2.}
$$

The given orthogonal-wave condition is therefore possible only at this forcing frequency. The upward [radiation condition](../../../../../../radiation-condition.md) excludes the $m=+\kappa$ branch.

Use [superposition](../../../../../../superposition-principle.md) with vertical amplitude $W$ in each component and [internal-wave polarization](../../../../../../internal-wave-polarization.md):

$$
\begin{aligned}
w_1&=W\cos(\kappa x-\kappa z-\omega t)+W\cos(-\kappa x-\kappa z-\omega t)\\
&=2W\cos(\kappa x)\cos(\kappa z+\omega t),\\
u_1&=W\cos(\kappa x-\kappa z-\omega t)-W\cos(-\kappa x-\kappa z-\omega t)\\
&=2W\sin(\kappa x)\sin(\kappa z+\omega t).
\end{aligned}
$$

The two sets of crests have slopes $+1$ and $-1$; their energy propagates upward and outward at angles of $45^\circ$, while their phases travel downward. Their interference makes fixed horizontal bands of vertical-velocity nodes, at $\cos\kappa x=0$, and horizontal-velocity nodes, at $\sin\kappa x=0$.

Put $A=\kappa x$, $B=\kappa z+\omega t$. The first-order displacement relative to mean parcel labels is

$$
\xi_1=-\frac{2W}{\omega}\sin A\cos B,\qquad
\zeta_1=\frac{2W}{\omega}\cos A\sin B.
$$

The horizontal displacement correction vanishes identically, while

$$
\xi_1w_{1x}+\zeta_1w_{1z}
=\frac{4\kappa W^2}{\omega}\left(\sin^2A\cos^2B-\cos^2A\sin^2B\right).
$$

Consequently the formal [cross-wave Stokes drift](../../../../../../cross-wave-stokes-drift.md) is

$$
\boxed{\mathbf u_s=\left(0,-\frac{2\kappa W^2}{\omega}\cos(2\kappa x)\right).}
$$

It has alternating downward and upward columns, no depth decay in this ideal infinite plane-wave field, and zero horizontal-period-averaged vertical transport. Each wave alone has zero drift; the interference terms create this result.

This calculation is a kinematic second-order consequence of the linear field, not a complete prediction of mean transport. In particular, an impermeable oscillating lower boundary cannot have that nonzero mean normal parcel velocity. Its first-order displacement is $\zeta_b=(2W/\omega)\cos(\kappa x)\sin\omega t$. Expanding the exact [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) on $z=\zeta_b$ gives

$$
w_2(x,0,t)=u_1(x,0,t)\,\partial_x\zeta_b-\zeta_b\,\partial_z w_1(x,0,t),
\qquad
\langle w_2(x,0,t)\rangle=\frac{2\kappa W^2}{\omega}\cos(2\kappa x).
$$

This [Eulerian mean velocity](../../../../../../eulerian-mean-flow.md) cancels the computed normal [Stokes drift](../../../../../../stokes-drift.md) at the material boundary. Away from it, the second-order mean-flow and buoyancy equations must also be satisfied. Thus the alternating drift is a valid formal cross-wave effect, but treating it alone as persistent transport with zero Eulerian mean would be physically incomplete. A prescribed permeable boundary would require its own second-order flux specification instead.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
