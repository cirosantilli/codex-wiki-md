<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a compact [Lie group](../../../../../../lie-group.md), take any positive-definite [Hermitian inner product](../../../../../../hermitian-form.md) $h_0$ on $V$ and average using probability [Haar measure](../../../../../../haar-measure.md):

$$
h(v,w)=\int_G h_0(gv,gw)\,dg.
$$

It remains positive definite, because the integrand is positive for a nonzero vector, and translation invariance makes it $G$-invariant. If $W\subset V$ is an [invariant subspace](../../../../../../invariant-subspace.md), then $W^\perp$ is invariant too: $h(gv,w)=h(v,g^{-1}w)=0$ when $v\in W^\perp$. Thus $V=W\oplus W^\perp$. Induction on dimension proves **complete reducibility**. This uses the usual continuous finite-dimensional representations of the [compact group](../../../../../../compact-group.md).

For a connected complex [reductive algebraic group](../../../../../../reductive-group.md), representations are understood to be [rational representations](../../../../../../rational-representation.md). Use a [compact real form](../../../../../../compact-real-form-of-a-complex-semisimple-lie-algebra.md) $K\subset G$ with $\operatorname{Lie}(G)=\operatorname{Lie}(K)\otimes_{\mathbb R}\mathbb C$. The structural construction takes a [compact real form](../../../../../../compact-real-form-of-a-complex-semisimple-lie-algebra.md) of the semisimple derived factor and the unit circles in the central torus, then passes through their finite central quotient. This is the compact-form structure of a complex reductive group, rather than an assumption that its given representation is already unitary.

The group $K$ is Zariski dense: the [Lie algebra](../../../../../../lie-algebra-split.md) of its Zariski closure contains the complex span of $\operatorname{Lie}(K)$, hence all of $\operatorname{Lie}(G)$; connectedness then makes that closure $G$. Average over $K$ as above. The [orthogonal complement](../../../../../../orthogonal-complement.md) of a $G$-[submodule](../../../../../../submodule.md) is $K$-invariant. Its stabilizer is a Zariski-closed subgroup, since preserving a fixed subspace is a system of algebraic matrix conditions. The stabilizer contains dense $K$, so it is all of $G$. This again gives an invariant complement to every [submodule](../../../../../../submodule.md) and proves

$$
\boxed{V\cong\bigoplus_j V_j\quad\text{with each }V_j\text{ irreducible}.}
$$

If reductivity is defined to allow finitely many components, first obtain a $G^0$-equivariant projection $P:V\to W$. Average its conjugates over the finite component group. Since $P$ commutes with $G^0$, the average is independent of coset representatives; it is $G$-equivariant and remains the identity on $W$. Its kernel supplies the required complement. Thus the result holds in that convention too.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
