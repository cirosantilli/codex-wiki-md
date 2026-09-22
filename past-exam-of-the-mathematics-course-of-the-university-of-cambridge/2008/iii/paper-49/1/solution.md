<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md), write $A_X=\operatorname{ad}X$ for its [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). The [Killing form](../../../../../killing-form.md) is the symmetric [bilinear form](../../../../../bilinear-form.md)

$$
\kappa(X,Y)=\operatorname{tr}(A_XA_Y).
$$

The [Jacobi identity](../../../../../jacobi-identity.md) gives $A_{[X,Y]}=[A_X,A_Y]$. Using the [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md),

$$
\kappa([X,Y],Z)=\operatorname{tr}([A_X,A_Y]A_Z)
=\operatorname{tr}(A_X[A_Y,A_Z])=\kappa(X,[Y,Z]).
$$

Thus it is an [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md). If $[T_a,T_b]=f_{ab}{}^cT_c$, the adjoint matrix has entries $(A_{T_a})^c{}_b=f_{ab}{}^c$. Its trace product yields the [structure constants of a Lie algebra](../../../../../structure-constant-of-a-lie-algebra.md) formula

$$
\boxed{\kappa_{ab}=\sum_{c,d}f_{ac}{}^d f_{bd}{}^c.}
$$

A [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) has zero [solvable radical](../../../../../radical-of-a-lie-algebra.md), equivalently no nonzero solvable ideal. In characteristic zero, the [Cartan criterion for semisimplicity](../../../../../cartan-criterion-for-semisimplicity.md) characterizes it by nondegeneracy of its [Killing form](../../../../../killing-form.md). A real [compact Lie algebra](../../../../../compact-lie-algebra.md) is the Lie algebra of a [compact Lie group](../../../../../compact-lie-group.md), equivalently one admitting a positive-definite invariant inner product. For a real semisimple algebra, the [compactness criterion from the Killing form](../../../../../compactness-criterion-from-the-killing-form.md) says compactness is equivalent to negative-definiteness of $\kappa$. An abelian compact-type algebra has zero Killing form, so this last characterization specifically concerns the semisimple case.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
