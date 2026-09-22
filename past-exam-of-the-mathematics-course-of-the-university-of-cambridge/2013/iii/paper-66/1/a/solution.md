<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $A>0$ and use primes for spatial derivatives. Two [integration by parts](../../../../../../integration-by-parts.md) operations in the first variation of the [elastic filament](../../../../../../elastic-filament.md)'s bending energy give

$$
\delta\mathcal E=A\int_0^L h''''\eta\,dx+A[h''\eta'-h'''\eta]_0^L.
$$

Thus the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) is $Ah''''=0$, and the fluctuation [differential operator](../../../../../../differential-operator.md) is $K=A\,d^4/dx^4$. In the [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) [inner product](../../../../../../inner-product.md), its boundary form is

$$
\langle u,Kv\rangle-\langle Ku,v\rangle=A[\overline u v'''-\overline{u'}v''+\overline{u''}v'-\overline{u'''}v]_0^L.
$$

The conjugate endpoint trace pairs are $(h,h''')$ and $(h',h'')$. Requiring one member of each pair to vanish gives the four standard [self-adjoint endpoint conditions for filament bending](../../../../../../self-adjoint-endpoint-conditions-for-filament-bending.md), applied at both ends:

- **Free-free:** $h''=h'''=0$. Both the bending [torque](../../../../../../torque.md) and the transverse endpoint [force](../../../../../../force.md) vanish; position and slope can vary.
- **Clamped-clamped:** $h=h'=0$. Position and slope are fixed, with reaction [forces](../../../../../../force.md) and [torques](../../../../../../torque.md) permitted. These are [clamped boundary conditions](../../../../../../clamped-boundary-condition.md).
- **Hinged-hinged:** $h=h''=0$. Position is fixed, but the endpoint rotates without bending [torque](../../../../../../torque.md).
- **Torqued-torqued:** $h'=h'''=0$. Slope is fixed by an endpoint [torque](../../../../../../torque.md), while translation is free and transverse [force](../../../../../../force.md) vanishes. The [torque](../../../../../../torque.md) is a reaction, not an additional condition setting $h''$ to zero.

Each pair annihilates the boundary form for all $u,v$ in the domain. Conversely, the remaining two endpoint traces can be chosen freely: requiring the boundary form to vanish against every such $u$ forces an adjoint-domain function $v$ to satisfy the same two conditions. This proves [self-adjointness](../../../../../../self-adjoint-operator.md), rather than just formal symmetry, on the corresponding fourth-order [Sobolev space](../../../../../../sobolev-space-split.md) domain.

The count four concerns these elementary homogeneous choices. **Identical-end [boundary conditions](../../../../../../boundary-condition.md) do not restrict all [self-adjoint operators](../../../../../../self-adjoint-operator.md) to these four possibilities.** For example, $h=0$, $h''=b h'$ at both ends, with any fixed real $b\ne0$, also annihilates the boundary form: the remaining expression is $-\overline{u'}b v'+b\overline{u'}v'=0$. This [Robin boundary condition](../../../../../../robin-boundary-condition.md) supplies a continuous family beyond the four listed pairs.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
