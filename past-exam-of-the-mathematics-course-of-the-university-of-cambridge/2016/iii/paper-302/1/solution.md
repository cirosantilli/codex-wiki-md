<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Over $\mathbb R$ or $\mathbb C$, a [Lie algebra](../../../../../lie-algebra-split.md) is a [vector space](../../../../../vector-space-split.md) with a [bilinear map](../../../../../bilinear-map.md) $[\ ,\ ]$ which is alternating and obeys the [Jacobi identity](../../../../../jacobi-identity.md):

$$
[X,X]=0,\qquad [X,[Y,Z]]+[Y,[Z,X]]+[Z,[X,Y]]=0.
$$

Bilinearity and alternation imply $[X,Y]=-[Y,X]$.

For a [Matrix Lie group](../../../../../matrix-lie-group.md), identify the [tangent space](../../../../../tangent-space.md) $\mathfrak g=T_I G$ with derivatives $\gamma'(0)$ of smooth curves through $I$. Product curves show that the sum of two such derivatives is again tangent, and reparametrization supplies scalar multiples. In particular this is a real [vector space](../../../../../vector-space-split.md), even when the matrices have complex entries. For $X,Y\in\mathfrak g$, choose a curve $\gamma(s)$ with $\gamma'(0)=X$. Conjugating a curve with derivative $Y$ shows that

$$
\gamma(s)Y\gamma(s)^{-1}\in\mathfrak g\qquad\text{for every sufficiently small }s.
$$

Differentiate this curve in the finite-dimensional [vector space](../../../../../vector-space-split.md) $\mathfrak g$. The result is

$$
\boxed{[X,Y]=XY-YX\in\mathfrak g.}
$$

The matrix [commutator](../../../../../commutator.md) is bilinear and alternating, and expanding the six terms proves its [Jacobi identity](../../../../../jacobi-identity.md). Thus this construction gives the [Lie algebra of a matrix Lie group](../../../../../lie-algebra-of-a-matrix-lie-group.md), with the appropriate bracket, using actual group curves rather than an assumed commutator closure.

For the [unitary group](../../../../../unitary-group.md), differentiating $\gamma(t)^\dagger\gamma(t)=I$ gives $X^\dagger+X=0$. Conversely, if $X^\dagger=-X$, then $e^{tX}$ is unitary and is a curve with derivative $X$. Consequently

$$
\boxed{\mathfrak u(N)=\{X:X^\dagger=-X\},\qquad\dim_{\mathbb R}\mathfrak u(N)=N^2.}
$$

This is the [unitary Lie algebra](../../../../../unitary-lie-algebra.md). The diagonal entries are purely imaginary, contributing $N$ real parameters, and each upper off-diagonal entry contributes two real parameters. A [matrix-unit basis of the unitary Lie algebra](../../../../../matrix-unit-basis-of-the-unitary-lie-algebra.md) is

$$
 iE^{(i,i)}\quad(1\leq i\leq N),\qquad E^{(i,j)}-E^{(j,i)},\quad i(E^{(i,j)}+E^{(j,i)})\quad(1\leq i<j\leq N).
$$

These $N+2\binom N2=N^2$ anti-Hermitian [matrix units](../../../../../matrix-unit.md) and their combinations are linearly independent over $\mathbb R$ and span every allowed entry.

The symplectic stabilizer is a [subgroup](../../../../../subgroup.md): the identity preserves $J$, and if $MJM^T=J$ and $NJN^T=J$, then

$$
(MN)J(MN)^T=M(NJN^T)M^T=J.
$$

Multiplying $MJM^T=J$ on the left by $M^{-1}$ and on the right by $M^{-T}$ gives $M^{-1}JM^{-T}=J$. Products and inverses remain unitary. This is the [compact symplectic group](../../../../../compact-symplectic-group.md), often denoted $USp(2n)$ or $Sp(n)$.

Differentiating the stabilizer equation gives $XJ+JX^T=0$. For $X=\begin{pmatrix}A&B\\C&D\end{pmatrix}$, this says

$$
B^T=B,\qquad C^T=C,\qquad D=-A^T.
$$

Together with $X^\dagger=-X$, these are equivalently

$$
\boxed{X=\begin{pmatrix}A&B\\-\overline B&\overline A\end{pmatrix},\qquad A^\dagger=-A,\quad B^T=B.}
$$

These conditions are also sufficient: $e^{tX}$ is unitary, and

$$
\frac{d}{dt}\bigl(e^{tX}Je^{tX^T}\bigr)=e^{tX}(XJ+JX^T)e^{tX^T}=0.
$$

Hence it stays in the subgroup. They characterize its [compact symplectic Lie algebra](../../../../../compact-symplectic-lie-algebra.md) without adding any trace condition. In fact the trace automatically vanishes. The free anti-Hermitian block $A$ has $n^2$ real parameters, and the complex [symmetric matrix](../../../../../symmetric-matrix.md) $B$ has $n(n+1)$ real parameters. Thus

$$
\boxed{\dim_{\mathbb R}\mathfrak h=n^2+n(n+1)=n(2n+1).}
$$

Here is a complete [matrix-unit basis of the compact symplectic Lie algebra](../../../../../matrix-unit-basis-of-the-compact-symplectic-lie-algebra.md). The generators supplying $A$ are

$$
H_i=i(E^{(i,i)}-E^{(i+n,i+n)})\quad(1\leq i\leq n),
$$



$$
P_{ij}=E^{(i,j)}-E^{(j,i)}+E^{(i+n,j+n)}-E^{(j+n,i+n)},
$$



$$
Q_{ij}=i\bigl(E^{(i,j)}+E^{(j,i)}-E^{(i+n,j+n)}-E^{(j+n,i+n)}\bigr)\quad(i<j).
$$

The two families supplying the real and imaginary parts of $B$ are, for $1\leq i\leq j\leq n$,

$$
U_{ij}=\frac{E^{(i,j+n)}+E^{(j,i+n)}-E^{(i+n,j)}-E^{(j+n,i)}}{1+\delta_{ij}},
$$



$$
V_{ij}=\frac{i\bigl(E^{(i,j+n)}+E^{(j,i+n)}+E^{(i+n,j)}+E^{(j+n,i)}\bigr)}{1+\delta_{ij}}.
$$

The denominator merely avoids double-counting diagonal entries. Each displayed generator obeys both defining tangent conditions. The $H,P,Q$ generators form a real basis of the allowed $A$ blocks, and the $U,V$ generators form a real basis of the complex symmetric $B$ blocks. Thus they are independent and their total number is $n(2n+1)$. **They give all generators required by the real compact algebra, including the case $n=1$.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
