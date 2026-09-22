<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Multiplying the matrices gives the [Heisenberg group](../../../../../heisenberg-group.md) law

$$
(x,y,z)(a,b,c)=(x+a,y+b,z+c+xb),\qquad
(x,y,z)^{-1}=(-x,-y,-z+xy).
$$

Differentiating at the identity gives all strictly upper-triangular matrices. With $X=E_{12}$, $Y=E_{23}$ and $Z=E_{13}$, the [commutator](../../../../../commutator.md) gives

$$
\boxed{\mathfrak g=\operatorname{span}\{X,Y,Z\},\qquad [X,Y]=Z,\quad [X,Z]=[Y,Z]=0.}
$$

This is the [Heisenberg Lie algebra](../../../../../heisenberg-lie-algebra.md).

The right [Maurer-Cartan form](../../../../../maurer-cartan-form.md) is

$$
dg\,g^{-1}=X\,dx+Y\,dy+Z\,(dz-y\,dx).
$$

Thus the [right-invariant coframe of the real Heisenberg group](../../../../../right-invariant-coframe-of-the-real-heisenberg-group.md) is $\sigma^1=dx$, $\sigma^2=dy$, $\sigma^3=dz-y\,dx$. Under a right translation,

$$
R_{(a,b,c)}(x,y,z)=(x+a,y+b,z+c+xb),
$$

we have $dx'=dx$, $dy'=dy$, and $dz'-y'dx'=dz-y\,dx$. All three [right-invariant differential forms](../../../../../right-invariant-differential-form.md) are preserved.

Every [right-invariant Riemannian metric](../../../../../right-invariant-riemannian-metric.md) is determined by an arbitrary [inner product](../../../../../inner-product.md) at the identity. In this coframe its most general expression is

$$
\boxed{h=H_{ij}\,\sigma^i\sigma^j,\qquad H=H^{\mathsf T}>0,\quad H_{ij}\text{ constant}.}
$$

Equivalently,

$$
\begin{aligned}
h={}&H_{11}dx^2+H_{22}dy^2+H_{33}(dz-y\,dx)^2\\
&+2H_{12}dx\,dy+2H_{13}dx(dz-y\,dx)+2H_{23}dy(dz-y\,dx).
\end{aligned}
$$

Products here are symmetric products. If a pseudo-Riemannian [metric tensor](../../../../../metric-tensor.md) is intended, replace positive definiteness by nondegeneracy. Since every right translation preserves the coframe, it is an [isometry](../../../../../isometry.md). The action is faithful, and $a\mapsto R_{a^{-1}}$ is a group homomorphism, embedding a copy of $G$ into the [isometry group](../../../../../isometry-group.md).

The one-parameter right translations produce the [Killing frame for a right-invariant Heisenberg metric](../../../../../killing-frame-for-a-right-invariant-heisenberg-metric.md):

$$
\boxed{K_X=\partial_x,\qquad K_Y=\partial_y+x\partial_z,\qquad K_Z=\partial_z.}
$$

Their flows are respectively $(x+t,y,z)$, $(x,y+t,z+xt)$ and $(x,y,z+t)$. Each preserves $h$, and their [Lie brackets of vector fields](../../../../../lie-bracket-of-vector-fields.md) are $[K_X,K_Y]=K_Z$, with the other two zero. This explicitly realizes the [Heisenberg Lie algebra](../../../../../heisenberg-lie-algebra.md). These [Killing vector fields](../../../../../killing-vector-field.md) are left-invariant vector fields; the vector fields dual to the right-invariant coframe are instead $\partial_x+y\partial_z,\partial_y,\partial_z$, and should not be substituted for these generators.

For the diagonal case, put

$$
h=\alpha\,dx^2+\beta\,dy^2+\chi(dz-y\,dx)^2,\qquad \alpha,\beta,\chi>0.
$$

The [Kaluza-Klein decomposition along a Killing field](../../../../../kaluza-klein-decomposition-along-a-killing-field.md) uses $V=h(K_X,K_X)=\alpha+\chi y^2$. Completing the square in $dx$ gives the [Heisenberg metric Kaluza-Klein reduction](../../../../../heisenberg-metric-kaluza-klein-reduction.md):

$$
\boxed{V=\alpha+\chi y^2,\qquad A=-\frac{\chi y}{\alpha+\chi y^2}\,dz,
\qquad \gamma=\beta\,dy^2+\frac{\alpha\chi}{\alpha+\chi y^2}\,dz^2.}
$$

These depend only on the quotient coordinates $(y,z)$ and satisfy $h=V(dx+A)^2+\gamma$. For a diagonal indefinite [metric tensor](../../../../../metric-tensor.md), the same expressions hold wherever $V\ne0$; a null [Killing vector field](../../../../../killing-vector-field.md) cannot be treated with this completed-square decomposition.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
