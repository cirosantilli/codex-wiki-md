<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [Lie derivative of a tensor field](../../../../../../lie-derivative-of-a-tensor-field.md), the scalar rule follows because a [vector field](../../../../../../vector-field.md) $X$ differentiates products of [smooth functions](../../../../../../smooth-function.md). On [vector fields](../../../../../../vector-field.md) the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) satisfies

$$
[X,fY]=f[X,Y]+X(f)Y.
$$

This follows by applying both sides to an arbitrary [smooth function](../../../../../../smooth-function.md) and expanding the two compositions of derivations. Both the scalar and vector-field operators are real-linear, so the extension theorem applies and gives the unique contraction-compatible tensor operator $\mathcal L_X$.

For a type-$(1,1)$ tensor $A$, regard it as the pointwise [endomorphism](../../../../../../endomorphism.md) of $TM$ obtained by contracting its covector slot with a vector. The [endomorphism-induced tensor derivation](../../../../../../endomorphism-induced-tensor-derivation.md) starts with

$$
D_Ah=0,\qquad D_AY=A(Y).
$$

It is real-linear and obeys $D_A(fY)=fA(Y)=fD_AY+(D_Af)Y$. The scalar operator zero is a derivation in every dimension, so there is no zero-dimensional obstruction here. Consequently it also extends uniquely. On a [differential one-form](../../../../../../one-form.md), the two operators are

$$
\boxed{(\mathcal L_X\omega)(Y)=X(\omega(Y))-\omega([X,Y]),
\qquad D_A\omega=-\omega\circ A.}
$$

Their actions on arbitrary [tensor fields](../../../../../../tensor-field.md) follow by the tensor-product rule; $D_A$ adds $A$ in every contravariant slot and subtracts its dual action in every covariant slot.

Functions in this calculation belong to $C^\infty(M)$: the printed $C^\infty(X)$ in Q2(c) is a typographical error. The contraction $C^1_2$ pairs the sole covector with the new vector $Y$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
