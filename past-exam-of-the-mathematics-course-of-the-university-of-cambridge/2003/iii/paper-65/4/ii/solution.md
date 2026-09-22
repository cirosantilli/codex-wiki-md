<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At fixed time write the azimuthal shift as $\delta=2AL_xt$ modulo $L_y$. Integrating a radial derivative over the box gives a boundary difference proportional to

$$
\int_0^{L_z}\int_0^{L_y}[Q(L_x,y,z)-Q(0,y,z)]\,dy\,dz
=\int_0^{L_z}\int_0^{L_y}[Q(0,y+\delta,z)-Q(0,y,z)]\,dy\,dz.
$$

The two integrals agree by translation invariance of an integral over a full azimuthal period. Hence $\langle\partial_xQ\rangle=0$. The ordinary periodic boundary conditions make the $y$ and $z$ boundary differences zero as well. Finally,

$$
\int_0^{L_y}x\partial_yQ\,dy=x[Q(x,L_y,z)-Q(x,0,z)]=0
$$

for every $x,z$. Thus the [volume averages in a shearing box](../../../../../../volume-averages-in-a-shearing-box.md) satisfy

$$
\boxed{\langle\partial_xQ\rangle=\langle\partial_yQ\rangle
=\langle x\partial_yQ\rangle=\langle\partial_zQ\rangle=0}.
$$

For smooth shearing-periodic extensions, spatial derivatives and products inherit the same [shearing-periodic boundary condition](../../../../../../shearing-periodic-boundary-condition.md). Their divergence therefore has zero [volume average](../../../../../../volume-average.md), and integration by parts is available without a residual boundary flux. Time differentiation of an average over this fixed physical box commutes with integration, even though the radial identification shifts with time.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
