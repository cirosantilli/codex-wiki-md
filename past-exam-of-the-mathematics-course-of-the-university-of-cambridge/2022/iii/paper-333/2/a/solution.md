<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $f>0$; replacing it by $|f|$ gives the thickness for either hemisphere. With $W=(u-U)+iv$, the steady anomaly equations reduce to

$$
\nu W''=ifW,
\qquad W(0)=-U,
\qquad W(\infty)=0.
$$

Thus the [Bottom Ekman layer](../../../../../../bottom-ekman-layer.md) has

$$
\boxed{\delta=\left(\frac{2\nu}{f}\right)^{1/2},quad
u=U[1-e^{-z/\delta}\cos(z/\delta)],quad
v=Ue^{-z/\delta}\sin(z/\delta).}
$$

Its integrated anomalous transport is

$$
\boxed{\mathbf u_T=\frac\delta2(-\mathbf U_g+\widehat{\mathbf z}\times\mathbf U_g).}
$$

It is the transport required by the vertically integrated momentum balance between Coriolis acceleration and bottom stress. For slowly varying geostrophic flow, $\nabla\cdot\mathbf U_g=0$ and $\nabla\cdot(\widehat z\times\mathbf U_g)=-\zeta_g$, so

$$
\nabla\cdot\mathbf u_T=-\frac\delta2\zeta_g.
$$

Mass conservation therefore gives the interior [Ekman pumping](../../../../../../ekman-pumping.md) condition

$$
\boxed{w(0^+)=\frac\delta2\zeta_g=\frac\delta2\nabla_h^2\psi.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
