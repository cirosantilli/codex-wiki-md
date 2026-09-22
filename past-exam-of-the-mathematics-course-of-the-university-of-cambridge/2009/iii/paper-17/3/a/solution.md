<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [left-invariant vector field](../../../../../../left-invariant-vector-field.md) $X$ on a [Lie group](../../../../../../lie-group.md) satisfies

$$
(dL_g)_h X_h=X_{gh}\qquad(g,h\in G),
$$

or equivalently $(L_g)_*X=X$ for every $g$. For $\xi\in T_eG$, define

$$
X^\xi_g=(dL_g)_e\xi.
$$

This is smooth because multiplication is smooth and its differential depends smoothly on the base points. The identity $L_g\circ L_h=L_{gh}$ gives $(dL_g)_hX^\xi_h=X^\xi_{gh}$, so $X^\xi$ is a [left-invariant vector field](../../../../../../left-invariant-vector-field.md). Conversely, left invariance forces any such field to have this form with $\xi=X_e$. Evaluation at $e$ and the construction above are inverse [linear maps](../../../../../../linear-map.md). Hence

$$
\boxed{T_eG\cong\{\text{left-invariant vector fields on }G\}.}
$$

The [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) is their [commutator](../../../../../../commutator.md) as [derivations](../../../../../../derivation-of-an-algebra.md) on [smooth functions](../../../../../../smooth-function.md): $[X,Y]f=X(Yf)-Y(Xf)$. It is another vector field because the cross terms cancel in the Leibniz rule for its action on a product. The bracket is preserved by a [diffeomorphism](../../../../../../diffeomorphism.md): conjugating the [derivation](../../../../../../derivation-of-an-algebra.md) operators by [pullback of a smooth function](../../../../../../pullback-of-a-smooth-function.md) preserves their [commutator](../../../../../../commutator.md). Therefore

$$
(L_g)_*[X,Y]=[(L_g)_*X,(L_g)_*Y]=[X,Y]
$$

for left-invariant $X,Y$. These fields are consequently closed under the bracket.

Transport the bracket to the [tangent space](../../../../../../tangent-space.md) by

$$
\boxed{[\xi,\eta]_{\mathfrak g}=[X^\xi,X^\eta]_e.}
$$

Bilinearity and antisymmetry come from the [commutator](../../../../../../commutator.md). The [Jacobi identity](../../../../../../jacobi-identity.md) follows by expanding the three nested [commutators](../../../../../../commutator.md) of [derivation](../../../../../../derivation-of-an-algebra.md) operators: their six terms cancel in pairs. Thus $T_eG$ is a [Lie algebra](../../../../../../lie-algebra-split.md), and the displayed correspondence is a [Lie algebra isomorphism](../../../../../../lie-algebra-isomorphism.md) onto the algebra of [left-invariant vector fields](../../../../../../left-invariant-vector-field.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
