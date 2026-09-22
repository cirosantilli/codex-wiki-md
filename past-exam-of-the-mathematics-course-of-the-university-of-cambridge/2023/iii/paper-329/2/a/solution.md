<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [long-wave approximation](../../../../../../long-wave-approximation.md) makes $u$ independent of $z$ at leading order. [Mass conservation](../../../../../../mass-conservation.md) and symmetry about $z=0$ then give

$$
u_x+w_z=0,
\qquad
\boxed{w=-zu_x}.
$$

For an incompressible Newtonian fluid,

$$
\sigma_{xx}=-p+2\mu u_x,
\qquad
\sigma_{zz}=-p+2\mu w_z=-p-2\mu u_x.
$$

The leading normal-stress balance on either surface is

$$
\boxed{\sigma_{zz}=-p_a+\gamma h_{xx}}.
$$

Since $\sigma_{xx}-\sigma_{zz}=4\mu u_x$, it follows that

$$
\boxed{\sigma_{xx}=-p_a+\gamma h_{xx}+4\mu u_x}.
$$

For a slice of length $\delta x$, the axial forces are the integrated normal stresses $2h\sigma_{xx}$ on its vertical ends, ambient pressure on the varying end height, and the horizontal components of [surface tension](../../../../../../surface-tension.md) on its two sloping faces. Expanding their difference to first order in $\delta x$ cancels the uniform $p_a$ terms and the lower-order capillary terms, leaving

$$
\boxed{
\frac\partial{\partial x}
\left(4\mu h\frac{\partial u}{\partial x}\right)
+\gamma h\frac{\partial^3h}{\partial x^3}=0}.
$$

The kinematic condition on $z=h(x,t)$ is $h_t+uh_x=w$. Substituting $w=-hu_x$ gives the second required relation,

$$
\boxed{h_t+(uh)_x=0}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
