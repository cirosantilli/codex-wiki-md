<h1 id="38a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the continuity equation to write the axial momentum equation in conservative form:

$$
\frac{\partial}{\partial z}(rw^2)
+\frac{\partial}{\partial r}(ruw)
=\nu\frac{\partial}{\partial r}\left(r\frac{\partial w}{\partial r}\right).
$$

Integrating from the axis to infinity, regularity at $r=0$ and decay of $u,w,w_r$ as $r\to\infty$ eliminate the boundary terms. Therefore the [conserved momentum flux of a laminar round jet](../../../../../../conserved-momentum-flux-of-a-laminar-round-jet.md) satisfies

$$
\boxed{\frac{dM}{dz}=0.}
$$

Let $W(z)$ be the centre-line velocity scale and $\delta(z)$ the jet width. Conservation gives $M\sim W^2\delta^2$, hence $W\delta\sim M^{1/2}$. The axial inertial and viscous terms scale as

$$
\frac{W^2}{z}\sim\frac{\nu W}{\delta^2},
$$

so $W\delta^2\sim\nu z$. Combining the two relations gives

$$
\boxed{\delta(z)\sim\frac{\nu z}{M^{1/2}},\qquad W(z)\sim\frac{M}{\nu z}.}
$$

Thus the width grows linearly and the centre-line speed decays as $z^{-1}$. The volume flux scales as

$$
Q(z)=\int_0^\infty rw\,dr\sim W\delta^2\sim\nu z,
$$

so it increases downstream. By [fluid entrainment](../../../../../../fluid-entrainment.md), the extra flux must be ambient fluid drawn radially into the jet.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38A](../../38a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
