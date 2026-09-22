<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the sign convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z.
$$

For the [Levi-Civita connection](../../../../../../levi-civita-connection.md) this is the [Riemannian curvature two-form](../../../../../../riemannian-curvature-two-form.md), an element of $\Omega^2(M;\operatorname{End}(TM))$: $R(X,Y)$ is an endomorphism of the [tangent bundle](../../../../../../tangent-bundle.md), alternating in $X,Y$, and the expression has [tensoriality](../../../../../../tensoriality.md) in all arguments. It is the [curvature form of a connection](../../../../../../curvature-form.md) for the tangent-bundle connection.

For the [first Bianchi identity](../../../../../../first-bianchi-identity.md), take the cyclic sum in $X,Y,Z$. Torsion-freeness says $\nabla_YZ-\nabla_ZY=[Y,Z]$, so the double-derivative terms combine to $\sum_{\mathrm{cyc}}\nabla_X[Y,Z]$. The remaining terms may be cyclically relabelled as $-\sum_{\mathrm{cyc}}\nabla_{[Y,Z]}X$. Using torsion-freeness once more, followed by the [Jacobi identity](../../../../../../jacobi-identity.md) for [vector fields](../../../../../../vector-field.md), gives

$$
\boxed{\sum_{\mathrm{cyc}}R(X,Y)Z
=\sum_{\mathrm{cyc}}[X,[Y,Z]]=0.}
$$

The [Ricci curvature](../../../../../../ricci-curvature.md) is the trace

$$
\operatorname{Ric}(Y,Z)=\sum_{a=1}^n\langle R(e_a,Y)Z,e_a\rangle
$$

for any [orthonormal basis](../../../../../../orthonormal-basis.md). The [sectional curvature](../../../../../../sectional-curvature.md) of the two-plane spanned by independent $u,v$ is

$$
K(u,v)=\frac{\langle R(u,v)v,u\rangle}{\|u\|^2\|v\|^2-\langle u,v\rangle^2}.
$$

These conventions give positive curvature on a round sphere. In dimension three, put $K_{ij}=K(e_i,e_j)$ and $r_i=\operatorname{Ric}(e_i,e_i)$. Curvature symmetries give

$$
r_1=K_{12}+K_{13},\qquad r_2=K_{12}+K_{23},\qquad r_3=K_{13}+K_{23}.
$$

Solving this linear system yields the [sectional curvatures from Ricci curvature in dimension three](../../../../../../sectional-curvatures-from-ricci-curvature-in-dimension-three.md) formula

$$
\boxed{K_{ij}=\frac{r_i+r_j-r_k}{2}
=r_i+r_j-\frac{\operatorname{Scal}}2\quad(\{i,j,k\}=\{1,2,3\}).}
$$

Here $\operatorname{Scal}=r_1+r_2+r_3$ is the [scalar curvature](../../../../../../scalar-curvature.md). The chosen [orthonormal basis](../../../../../../orthonormal-basis.md) need not diagonalize Ricci; its diagonal evaluations already determine these three sectional curvatures.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 131](../../../paper-131-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
