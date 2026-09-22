<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The displayed matrices describe the orientation-preserving component $SE(2)$ of the full [Euclidean group](../../../../../euclidean-group.md) $E(2)=O(2)\ltimes\mathbb R^2$. Both have the same [Lie algebra](../../../../../lie-algebra-split.md), so this naming convention does not affect the calculation. Choose the translation generators $P_1,P_2$ and rotation generator $J$ in the [Lie algebra](../../../../../lie-algebra-split.md) of this [Matrix Lie group](../../../../../matrix-lie-group.md) as

$$
P_1=\begin{pmatrix}0&0&1\\0&0&0\\0&0&0\end{pmatrix},\qquad P_2=\begin{pmatrix}0&0&0\\0&0&1\\0&0&0\end{pmatrix},\qquad J=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&0\end{pmatrix}.
$$

Taking matrix [commutators](../../../../../commutator.md) gives

$$
\boxed{[P_1,P_2]=0,\qquad[J,P_1]=P_2,\qquad[J,P_2]=-P_1.}
$$

All remaining brackets follow from antisymmetry. The corresponding [left-invariant vector fields](../../../../../left-invariant-vector-field.md) in coordinates $(x,y,\psi)$ are

$$
L_1=\cos\psi\,\partial_x+\sin\psi\,\partial_y,\qquad L_2=-\sin\psi\,\partial_x+\cos\psi\,\partial_y,\qquad L_3=\partial_\psi.
$$

Their [Lie brackets of vector fields](../../../../../lie-bracket-of-vector-fields.md) obey the same relations. This also fixes which sign of the rotation generator is being used.

There is an important qualification to the printed connection prescription. For an arbitrary [vector field](../../../../../vector-field.md) $Z$ and smooth function $f$, its literal right-hand side obeys

$$
\lambda[L_i,fZ]=\lambda L_i(f)Z+\lambda f[L_i,Z].
$$

An [affine connection](../../../../../affine-connection.md) instead requires $\nabla_{L_i}(fZ)=L_i(f)Z+f\nabla_{L_i}Z$. Thus **the formula for arbitrary $Z$ defines a connection only when $\lambda=1$**. For example, at $\psi=0$, take $i=1$, $f=x$ and $Z=L_1$: the erroneous formula gives $\lambda L_1$, whereas the [Leibniz rule](../../../../../leibniz-rule.md) requires $L_1$.

The intended one-parameter family is the [bracket connection on a Lie group](../../../../../bracket-connection-on-a-lie-group.md): prescribe the rule for left-invariant $Z$, then extend it by the [Leibniz rule](../../../../../leibniz-rule.md). If $[L_i,L_j]=c_{ij}{}^kL_k$, this means

$$
\nabla_{L_i}L_j=\lambda c_{ij}{}^kL_k,\qquad \nabla_{L_i}(z^jL_j)=L_i(z^j)L_j+\lambda z^j c_{ij}{}^kL_k.
$$

Extend linearly over functions in the first slot. This is a well-defined [affine connection](../../../../../affine-connection.md) for every real $\lambda$. The following [Ricci tensor](../../../../../ricci-tensor.md) calculation applies to this intended family; under the literal arbitrary-$Z$ reading only its $\lambda=1$ member exists.

Use the curvature convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z,\qquad \operatorname{Ric}(X,Y)=\operatorname{tr}\bigl(Z\mapsto R(Z,X)Y\bigr).
$$

For [left-invariant vector fields](../../../../../left-invariant-vector-field.md) the [structure constants of a Lie algebra](../../../../../structure-constant-of-a-lie-algebra.md) are constant. The [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
\begin{aligned}
R(X,Y)Z&=\lambda^2\bigl([X,[Y,Z]]-[Y,[X,Z]]\bigr)-\lambda[[X,Y],Z]\\
&=\lambda(\lambda-1)[[X,Y],Z].
\end{aligned}
$$

Writing $A=\lambda(\lambda-1)$, the only nonzero curvature actions, apart from antisymmetry in the first two slots, are

$$
R(L_3,L_1)L_3=A L_1,\qquad R(L_3,L_2)L_3=A L_2.
$$

For instance, $[[J,P_1],J]=[P_2,J]=P_1$. Contracting the first and output slots gives $\operatorname{Ric}(L_3,L_3)=-2A$, while every other component vanishes. Equivalently, $[[Z,X],Y]=\operatorname{ad}_Y\operatorname{ad}_X Z$, so

$$
\operatorname{Ric}(X,Y)=A\,B(X,Y),\qquad B(X,Y)=\operatorname{tr}(\operatorname{ad}_X\operatorname{ad}_Y).
$$

This is the [Killing form](../../../../../killing-form.md). Here $\operatorname{ad}_J$ rotates the two-dimensional translation space and vanishes on $J$, so $B(J,J)=-2$; translation generators give all other components zero. Therefore

$$
\boxed{(\operatorname{Ric}_{ij})_{i,j=1}^3=\begin{pmatrix}0&0&0\\0&0&0\\0&0&2\lambda(1-\lambda)\end{pmatrix}.}
$$

Since the coframe component dual to $L_3$ is $d\psi$, the same [Ricci tensor](../../../../../ricci-tensor.md) is $2\lambda(1-\lambda)d\psi\otimes d\psi$ in these coordinates. Reversing the curvature convention reverses this sign.

At both $\lambda=0$ and $\lambda=1$, the full curvature vanishes. At $\lambda=0$, the [left-invariant vector fields](../../../../../left-invariant-vector-field.md) form a global [parallel frame](../../../../../parallel-frame-along-a-curve.md). At $\lambda=1$, every [right-invariant vector field](../../../../../right-invariant-vector-field.md) is parallel because left- and right-invariant [vector fields](../../../../../vector-field.md) commute; the connection is flat in that global [parallel frame](../../../../../parallel-frame-along-a-curve.md). Flatness does not imply zero torsion: for left-invariant arguments the [torsion tensor](../../../../../torsion-tensor.md) is

$$
T(X,Y)=\nabla_XY-\nabla_YX-[X,Y]=(2\lambda-1)[X,Y].
$$

Thus **the two endpoint connections are flat, with opposite nonzero torsion**. For comparison, $\lambda=1/2$ is torsion-free but has nonzero curvature, with $\operatorname{Ric}_{33}=1/2$. No metric has been specified, so these connections should not automatically be identified with a [Levi-Civita connection](../../../../../levi-civita-connection.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
