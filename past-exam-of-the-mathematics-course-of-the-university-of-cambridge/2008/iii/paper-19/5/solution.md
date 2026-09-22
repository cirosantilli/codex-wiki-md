<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the [Riemannian curvature two-form](../../../../../riemannian-curvature-two-form.md) convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z,
$$

and define its four-covariant [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) by $R(X,Y,Z,W)=g(R(X,Y)W,Z)$. This makes $R(X,Y,X,Y)$ positive on an orthonormal two-plane of the unit sphere. The full algebraic symmetries are

$$
\begin{aligned}
R(X,Y,Z,W)&=-R(Y,X,Z,W),\\
R(X,Y,Z,W)&=-R(X,Y,W,Z),\\
R(X,Y,Z,W)&=R(Z,W,X,Y),\\
R(X,Y,Z,W)+R(Y,Z,X,W)+R(Z,X,Y,W)&=0.
\end{aligned}
$$

Together with multilinearity, these are antisymmetry in each pair, interchange of pairs, and the [first Bianchi identity](../../../../../first-bianchi-identity.md).

Define the [Ricci tensor](../../../../../ricci-tensor.md) by the basis-independent contraction

$$
\operatorname{Ric}(Y,W)=\operatorname{tr}\bigl(v\mapsto R(v,Y)W\bigr)=\sum_{a=1}^nR(e_a,Y,e_a,W)
$$

for any orthonormal basis $(e_a)$. The trace is invariant under change of basis, and contraction of the smooth curvature tensor gives a smooth covariant two-tensor. Pair interchange gives $R(e_a,Y,e_a,W)=R(e_a,W,e_a,Y)$, so $\operatorname{Ric}(Y,W)=\operatorname{Ric}(W,Y)$. Thus **the Ricci tensor is a symmetric covariant 2-tensor**.

The [sectional curvature](../../../../../sectional-curvature.md) of the two-plane $\sigma=\operatorname{span}(u,v)$ is

$$
K(\sigma)=\frac{R(u,v,u,v)}{g(u,u)g(v,v)-g(u,v)^2}.
$$

Both numerator and denominator multiply by the square of the determinant under a change of basis of $\sigma$, so this is a plane invariant. The directional [Ricci curvature](../../../../../ricci-curvature.md) of $u\ne0$ is $\operatorname{Ric}(u,u)/g(u,u)$. For an orthonormal basis beginning with $u/|u|$, it equals the sum of the sectional curvatures of the planes containing that basis vector.

In dimension three, suppose this directional value is $c$ at the point under consideration. For any orthonormal triple $(e_1,e_2,e_3)$, put $K_{ij}=K(\operatorname{span}(e_i,e_j))$. Then

$$
K_{12}+K_{13}=c,\qquad K_{12}+K_{23}=c,\qquad K_{13}+K_{23}=c,
$$

so all three are $c/2$. Every two-plane can be the span of the first two members of such a triple. Consequently

$$
\boxed{\text{isotropic Ricci curvature }c\text{ in dimension }3\ \Longrightarrow\ K(\sigma)=c/2\text{ for every plane at that point}.}
$$

This is a pointwise conclusion, as required; it uses [sectional curvatures from Ricci curvature in dimension three](../../../../../sectional-curvatures-from-ricci-curvature-in-dimension-three.md) and asserts no spatial constancy.

For the product, the canonical identification $T_{(p,q)}(M\times N)=T_pM\oplus T_qN$ defines the [product Riemannian metric](../../../../../product-riemannian-metric.md)

$$
g_{(p,q)}((u,v),(u',v'))=g_M(u,u')+g_N(v,v').
$$

It is smooth in product charts and positive definite, since a nonzero vector has a nonzero component in at least one factor. Those components are orthogonal. The coordinate connection computation in the subparts below gives

$$
R^{M\times N}((u_1,u_2),(v_1,v_2))(w_1,w_2)=\bigl(R^M(u_1,v_1)w_1,R^N(u_2,v_2)w_2\bigr).
$$

Taking the trace in orthonormal bases of the two factors therefore gives $\operatorname{Ric}_{M\times N}=\operatorname{Ric}_M\oplus\operatorname{Ric}_N$.

For the final example choose the two round unit spheres. Each has sectional curvature one and Ricci tensor equal to its metric. Hence the product has $\operatorname{Ric}=g$, so every directional Ricci curvature is one. A two-plane tangent to one factor has sectional curvature one, whereas a mixed two-plane has sectional curvature zero by (iii). This gives [constant Ricci curvature without constant sectional curvature](../../../../../constant-ricci-curvature-without-constant-sectional-curvature.md):

$$
\boxed{(S^2\times S^2,g_{S^2}\oplus g_{S^2}):\quad\operatorname{Ric}(v,v)/|v|^2=1,\quad K_{\mathrm{factor}}=1,\quad K_{\mathrm{mixed}}=0.}
$$

Both kinds of plane occur at every point, so the sectional curvatures fail to be constant even at a single point.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
