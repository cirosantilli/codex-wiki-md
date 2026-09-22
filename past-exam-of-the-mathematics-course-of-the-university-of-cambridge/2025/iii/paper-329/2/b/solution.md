<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The broad faces have curvature zero to leading order, so their [stress boundary condition](../../../../../../stress-boundary-condition.md) gives $\sigma_{xx}=-p_e$. The semicircular edges have curvature $1/h$, giving $\sigma_{yy}=-p_e-\gamma/h$. [Incompressible flow](../../../../../../incompressible-flow.md) gives $u_x+v_y+w_z=0$; uniform transverse normal stresses imply uniform transverse extension rates, and eliminating them from the [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) yields

$$
\boxed{\sigma_{zz}=-p_e-\frac{\gamma}{2h}+3\mu w'.}
$$

At an edge, the [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) balances axial advection of $b$, lateral strain, and capillary retraction. This gives

$$
\boxed{wb'+\frac b2w'+\frac{\gamma b}{4\mu h}=0.}
$$

The equation $hbw=Q$ expresses conservation of volume flux, while

$$
3\mu hbw'+\frac{\gamma b}{2}=F
$$

states that the total axial tension is constant. Define

$$
\boxed{\Gamma=\frac\gamma{\mu Q},
\qquad T=\frac F{\mu Q}.}
$$

Then $[\Gamma]=L^{-2}$ and $[T]=L^{-1}$, and substitution of $h=Q/(bw)$ gives

$$
\frac{b'}b+\frac12\frac{w'}w=-\frac{\Gamma b}{4},
\qquad
3\frac{w'}w=-\frac{\Gamma b}{2}+T.
$$

Subtracting these logarithmic-derivative equations gives

$$
\left(\log\frac wb\right)'=\frac T2,
\qquad
\boxed{w(z)=\frac{w(0)}{b_0},b(z)e^{Tz/2}.}
$$

The remaining width equation is

$$
\frac{b'}b=-\frac{\Gamma b+T}{6}.
$$

Thus, for $T\ne0$,

$$
\boxed{
\frac1{b(z)}=\frac{e^{Tz/6}}{b_0}
+\frac\Gamma T\left(e^{Tz/6}-1\right),}
$$

while the continuous $T=0$ limit is $1/b=1/b_0+\Gamma z/6$.

If $\Gamma=0$, then $b/b_0=e^{-Tz/6}$, $w/w(0)=e^{Tz/3}$, and [mass conservation](../../../../../../mass-conservation.md) gives $h/h(0)=e^{-Tz/6}$. Therefore a prescribed thinning ratio $R=h(L)/h(0)$ requires

$$
\boxed{F=\mu QT
=\frac{6\mu Q}{L}\log\frac{h(0)}{h(L)}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
