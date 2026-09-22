<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [elastic filament](../../../../../../elastic-filament.md), apply a variation $\eta(x)$. Two [integration by parts](../../../../../../integration-by-parts.md) operations give

$$
\delta\mathcal E=A\int_0^L h''\eta''dx
=A\int_0^L h^{(4)}\eta\,dx
+A[h''\eta'-h^{(3)}\eta]_0^L.
$$

At a free endpoint both $\eta$ and $\eta'$ are arbitrary. The [free-end bending boundary conditions](../../../../../../free-end-bending-boundary-conditions.md) and the unloaded [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) are therefore

$$
\boxed{h^{(4)}=0\quad(0<x<L),\qquad
h''=h^{(3)}=0\quad\text{at }x=0,L.}
$$

Here $Ah''$ is the bending moment and $-Ah^{(3)}$ the transverse shear-force convention. The equilibrium shapes are affine, reflecting free translation and tilt.

On $L^2(0,L)$ define $K=A\partial_x^4$ on $H^4$ functions obeying those endpoints. The [self-adjoint endpoint conditions for filament bending](../../../../../../self-adjoint-endpoint-conditions-for-filament-bending.md) annul the boundary form

$$
\langle u,Kv\rangle-\langle Ku,v\rangle
=A[\overline u v^{(3)}-\overline{u'}v''+\overline{u''}v'-\overline{u^{(3)}}v]_0^L.
$$

This proves symmetry. To establish actual [self-adjointness](../../../../../../self-adjoint-operator.md), the adjoint-domain boundary form must vanish for every free-end $u$. The endpoint values $u,u'$ can be varied independently, forcing $v''=v^{(3)}=0$ at both ends. The regular fourth-order expression then gives the same $H^4$ domain for the adjoint. Thus the domains coincide and $K$ is [self-adjoint](../../../../../../self-adjoint-operator.md). Also $\langle h,Kh\rangle=A\int|h''|^2dx\geq0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
