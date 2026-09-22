<h1 id="4b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [quotient theorem for Cartesian tensors](../../../../../../quotient-theorem-for-cartesian-tensors.md) here says: if contracting $T_{ij}$ with every [vector](../../../../../../vector.md) $v_j$ gives the components $w_i=T_{ij}v_j$ of a [vector](../../../../../../vector.md) in every right-handed [orthonormal basis](../../../../../../orthonormal-basis.md), then $T$ obeys the second-order [tensor](../../../../../../tensor.md) transformation law. Conversely that transformation law guarantees the contraction is a [vector](../../../../../../vector.md). One may equivalently test that $u_iT_{ij}v_j$ is a [scalar](../../../../../../scalar.md) for every pair of [vectors](../../../../../../vector.md) $u,v$.

By part (a), $v'=Rv$ and $w'=Rw$. The contraction property in the new [basis](../../../../../../basis.md) says

$$
T'Rv=w'=Rw=RTv.
$$

Since this holds for every test [vector](../../../../../../vector.md), $T'R=RT$. Using $R^{-1}=R^T$ gives

$$
\boxed{T'=RTR^T,\qquad T'_{ij}=R_{ik}R_{j\ell}T_{k\ell}.}
$$

For the converse, $T'v'=RTR^TRv=RTv=Rw$, exactly the [vector](../../../../../../vector.md) law. For the equivalent [scalar](../../../../../../scalar.md) formulation, invariance of $u^TTv$ for every $u,v$ gives $u^TR^TT'Rv=u^TTv$, forcing the same [matrix](../../../../../../matrix.md) identity.

The quantifier “every” matters: an arbitrary nonzero [matrix](../../../../../../matrix.md) can annihilate one fixed [vector](../../../../../../vector.md), so a single successful contraction cannot establish tensoriality. The stated [bases](../../../../../../basis.md) test proper rotations; transformation under [orthogonal reflections](../../../../../../reflection-in-a-hyperplane.md) would require an additional hypothesis if that were wanted. “Second-order” counts tensor indices, rather than the [matrix rank](../../../../../../matrix-rank.md) of a particular component [matrix](../../../../../../matrix.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4B](../../4b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
