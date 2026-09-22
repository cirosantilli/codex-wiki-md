# Cross-product Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra-split.md)

The [vector space](vector-space-split.md) $\mathbb R^3$ with the [cross product](cross-product.md) as [Lie bracket](lie-bracket.md), $[x,y]=x\times y$. Bilinearity and $x\times x=0$ give an [Alternating Lie bracket](alternating-lie-bracket.md); the [vector triple product identity](vector-triple-product.md) proves the [Jacobi identity](jacobi-identity.md) because the three expressions $x\times(y\times z)=y(x\cdot z)-z(x\cdot y)$ cancel cyclically, using the symmetric [dot product](dot-product.md).

Its relation to the [SO(3) Lie algebra](so-3-lie-algebra.md) is explicit. For a [vector](vector.md) $x=(x_1,x_2,x_3)$, define the [skew-symmetric matrix](skew-symmetric-matrix.md)

$$
\widehat{x}=\begin{pmatrix}0&-x_3&x_2\\x_3&0&-x_1\\-x_2&x_1&0\end{pmatrix},\qquad \widehat{x}v=x\times v.
$$

Then $[\widehat{x},\widehat{y}]=\widehat{x\times y}$: acting on $v$, the left side is $x\times(y\times v)-y\times(x\times v)=(x\times y)\times v$. Every real $3\times3$ [skew-symmetric matrix](skew-symmetric-matrix.md) occurs uniquely, so this hat map is a [Lie algebra isomorphism](lie-algebra-isomorphism.md). With the standard [basis vectors](basis-vector.md) $e_1,e_2,e_3$,

$$
X=\widehat{e_1}=\begin{pmatrix}0&0&0\\0&0&-1\\0&1&0\end{pmatrix},\quad Y=\widehat{e_2}=\begin{pmatrix}0&0&1\\0&0&0\\-1&0&0\end{pmatrix},\quad Z=\widehat{e_3}=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&0\end{pmatrix},
$$

and their [matrix commutators](commutator.md) are $[X,Y]=Z$, $[Y,Z]=X$, $[Z,X]=Y$. With active [rotation matrices](rotation-matrix.md) acting on column [vectors](vector.md), $\exp(t\widehat{x})$ rotates through angle $t\lVert x\rVert$ about the oriented axis $x$ when $x\ne0$. In particular $\exp(tZ)e_1=(\cos t,\sin t,0)$, fixing the positive-angle convention used in the [small rotation commutator](small-rotation-commutator.md).

The map $x\mapsto-(i/2)x\cdot\sigma$ is also a [Lie algebra isomorphism](lie-algebra-isomorphism.md) to the compact real [SU(2) Lie algebra](su-2-lie-algebra.md), using the [Pauli matrix commutator identity](pauli-matrix-commutator-identity.md). These two identifications concern [Lie algebras](lie-algebra-split.md); they do not identify the corresponding [Lie groups](lie-group.md) globally.

## ↑ Ancestors (7)

1. [Lie algebra](lie-algebra-split.md)
2. [Lie theory](lie-theory-split.md)
3. [Diagonal dominance](diagonal-dominance.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Jacobi identity](jacobi-identity.md)
- [Lie bracket](lie-bracket.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-41/1/solution.md)
- [Small rotation commutator](small-rotation-commutator.md)
