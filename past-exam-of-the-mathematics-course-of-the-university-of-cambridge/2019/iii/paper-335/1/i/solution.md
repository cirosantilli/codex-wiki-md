<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [outgoing Green function for the three-dimensional Helmholtz equation](../../../../../../outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md)

$$
G_k(\mathbf r,\mathbf r')=\frac{e^{ik|\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|},\qquad (\Delta_{\mathbf r'}+k^2)G_k=-\delta_{\mathbf r}.
$$

Let $\mathbf n'$ point out of the obstacle $D$ into the exterior. Apply [Green second identity](../../../../../../green-second-identity.md) to the field and $G_k$ in a large exterior region. Their [Sommerfeld radiation conditions](../../../../../../sommerfeld-radiation-condition.md) make the outer-sphere contribution vanish. The normal on the exterior region's inner boundary is $-\mathbf n'$, so the [Kirchhoff–Helmholtz representation](../../../../../../kirchhoff-helmholtz-representation.md) is

$$
\boxed{\psi(\mathbf r)=\int_VG_k(\mathbf r,\mathbf r')Q(\mathbf r')\,d\mathbf r'+\int_{\partial D}[\psi(\mathbf r')\partial_{n'}G_k-G_k\partial_{n'}\psi(\mathbf r')]\,dS',\quad\mathbf r\notin\overline D.}
$$

The first integral is the incident source field $\psi_i$. Therefore the scattered field is the surface term. Since $\psi_i$ solves the homogeneous [Helmholtz equation](../../../../../../helmholtz-equation.md) within the obstacle, its surface term is zero at exterior observation points; the same representation can be written using only scattered-field traces:

$$
\boxed{\psi_s(\mathbf r)=\int_{\partial D}[\psi_s\partial_{n'}G_k-G_k\partial_{n'}\psi_s]\,dS'.}
$$

The unknown boundary condition determines these traces, but the representation itself does not require choosing that condition.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
