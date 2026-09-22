<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the embedded [Lie group](../../../../../../lie-group.md), the [tangent space](../../../../../../tangent-space.md) $T_eG$ consists of velocities $\gamma'(0)$ of smooth curves in $G$ satisfying $\gamma(0)=e$. The ambient coordinates identify these velocities with vectors in $\mathbb R^n$, but the tangent space itself is intrinsic. Let $c_g(a)=gag^{-1}$. Since this conjugation map fixes $e$, its derivative defines the [Adjoint representation of a Lie group](../../../../../../adjoint-representation-of-a-lie-group.md):

$$
\boxed{\operatorname{Ad}_g=(dc_g)_e:T_eG\to T_eG.}
$$

The inverse is $\operatorname{Ad}_{g^{-1}}$, and $c_{gh}=c_g\circ c_h$ gives $\operatorname{Ad}_{gh}=\operatorname{Ad}_g\operatorname{Ad}_h$. Thus this is a smooth group homomorphism into the linear automorphisms of $T_eG$.

Differentiate that representation at the identity. The tangent space of $GL(T_eG)$ at its identity is $\operatorname{End}(T_eG)$, so $\operatorname{ad}=(d\operatorname{Ad})_e$ is a linear map from $T_eG$ into those endomorphisms. The [Lie bracket](../../../../../../lie-bracket.md) is

$$
\boxed{[X,Y]=\operatorname{ad}(X)Y=\left.\frac d{ds}\right|_{s=0}\operatorname{Ad}_{\gamma(s)}Y,\quad\gamma(0)=e,\quad\gamma'(0)=X.}
$$

Equivalently, if $\eta(0)=e$ and $\eta'(0)=Y$, this is the mixed derivative at $(0,0)$ of $\gamma(s)\eta(t)\gamma(s)^{-1}$ in ambient coordinates. For a matrix [Lie group](../../../../../../lie-group.md), conjugation is ordinary matrix conjugation and this formula reduces to $[X,Y]=XY-YX$.

The checks required are that the derivative is independent of the representing curves, that it is bilinear and alternating, and that it satisfies the [Jacobi identity](../../../../../../jacobi-identity.md). One must also check that each $\operatorname{Ad}_g$ preserves this bracket. Equivalently identify $X$ with its left-invariant vector field $X^L(g)=(dL_g)_eX$; the bracket above agrees with the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) at $e$. These checks make $T_eG$ a [Lie algebra](../../../../../../lie-algebra-split.md) and upgrade the adjoint maps to its Lie algebra automorphisms.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
