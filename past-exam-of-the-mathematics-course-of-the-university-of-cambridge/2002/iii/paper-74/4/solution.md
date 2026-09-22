<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Define the raw [Killing form](../../../../../killing-form.md) by

$$
\boxed{K(X,Y)=\operatorname{Tr}(\operatorname{ad}X\operatorname{ad}Y).}
$$

For a finite-dimensional real or complex [Lie algebra](../../../../../lie-algebra-split.md) in characteristic zero, it is nondegenerate exactly when the algebra is a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md). For a real compact semisimple algebra it is negative definite. Consequently the positive compact Killing metric is $g=-K$: for example on $\mathfrak{su}(2)$ with $[e_i,e_j]=\varepsilon_{ijk}e_k$, $K_{ij}=-2\delta_{ij}$ and $-K$ gives a [Riemannian metric](../../../../../riemannian-metric.md) on $SU(2)$. An overall minus sign in the term “Killing metric” is common here; raw trace $K$ itself is negative definite in this example.

For a [Lorentzian metric](../../../../../lorentzian-metric.md) use $\mathfrak{sl}(2,\mathbb R)$ with $[h,e]=2e$, $[h,f]=-2f$, $[e,f]=h$. Direct traces give

$$
K_{(h,e,f)}=\begin{pmatrix}8&0&0\\0&0&4\\0&4&0\end{pmatrix},
$$

whose [metric signature](../../../../../metric-signature.md) is $(2,1)$. For a non-Abelian degenerate example, the three-dimensional [Heisenberg Lie algebra](../../../../../heisenberg-lie-algebra.md) has $[x,y]=z$ central. Every product of two adjoint maps is zero, so $K=0$.

For any adjoint-invariant nondegenerate metric on a [Lie group](../../../../../lie-group.md), the [Koszul formula](../../../../../koszul-formula.md) on left-invariant fields simplifies to

$$
2g(\nabla_XY,Z)=g([X,Y],Z),\qquad
\boxed{\nabla_XY=\frac12[X,Y].}
$$

Take $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$. The [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
R(X,Y)Z=\frac14\bigl([X,[Y,Z]]-[Y,[X,Z]]\bigr)-\frac12[[X,Y],Z]
=-\frac14[[X,Y],Z].
$$

Taking the trace of $Z\mapsto R(Z,X)Y=-\operatorname{ad}Y\operatorname{ad}X(Z)/4$ yields

$$
\boxed{\operatorname{Ric}(X,Y)=-\frac14K(X,Y).}
$$

Thus the metric $g=K$ is a [Killing-form Einstein metric](../../../../../killing-form-einstein-metric.md) with Einstein constant $-1/4$. With $g=-K$ the same connection has constant $+1/4$. This proves the [Einstein manifold](../../../../../einstein-manifold.md) assertion for every semisimple group, including products when the unscaled Killing form is used on all factors.

There is also a different, flat metric-preserving connection. Declare the global left-invariant frame parallel:

$$
D_X(Y^ae_a)=X(Y^a)e_a.
$$

Its curvature is zero because applying two derivatives to coefficient functions and subtracting their commutator gives zero. Its metric derivative vanishes since $g_{ab}$ is constant in this frame. Its [torsion tensor](../../../../../torsion-tensor.md) on invariant fields is

$$
\boxed{T(e_a,e_c)=-[e_a,e_c],\qquad T_a{}^b{}_c=-C_a{}^b{}_c.}
$$

For each fixed $c$, antisymmetry gives $T_a{}^b{}_c=C_c{}^b{}_a$, so this is the matrix of $\operatorname{ad}e_c$. The [torsion contractions of a left-parallel Lie-group connection](../../../../../torsion-contractions-of-a-left-parallel-lie-group-connection.md) therefore are

$$
\boxed{T_a{}^a{}_c=\operatorname{Tr}(\operatorname{ad}e_c)=0,\qquad
T_a{}^b{}_cT_b{}^a{}_d=K_{cd}.}
$$

The zero trace follows because a semisimple algebra is perfect: every element is a sum of brackets, and the adjoint of a bracket is a matrix commutator with zero trace. If the metric convention is $g=-K$, the second contraction is $-g_{cd}$. These [flat translation connections on a Lie group](../../../../../flat-translation-connections-on-a-lie-group.md) are not the torsion-free [Levi-Civita connection](../../../../../levi-civita-connection.md); nonzero torsion permits flatness alongside the curved Killing metric.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
