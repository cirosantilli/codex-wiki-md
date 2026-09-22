<h1 id="9g/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Induct on $n$. The one-dimensional assertion is immediate, and the zero-dimensional case is vacuous. If $T$ has a [cyclic vector](../../../../../../cyclic-vector.md) spanning all of $V$, the direct proof in part (ii) applies. Otherwise choose $x\ne0$ and let $W$ be its [cyclic subspace](../../../../../../cyclic-subspace.md). Part (i) makes $W$ invariant; the absence of a cyclic vector makes it proper and nonzero.

By induction, the restriction to $W$ is annihilated by $\chi_A$, and the induced map on $V/W$ is annihilated by $\chi_D$. The quotient assertion means $\chi_D(T)V\subset W$. Applying the restriction assertion next gives

$$
\chi_A(T)\chi_D(T)V=0.
$$

By the characteristic factorization in part (iii), this is precisely $\chi_T(T)V=0$. Hence

$$
\boxed{\chi_T(T)=0\quad\text{for every finite-dimensional endomorphism}.}
$$

This is the [Cayley-Hamilton theorem from cyclic subspaces](../../../../../../cayley-hamilton-theorem-from-cyclic-subspaces.md); using the quotient map is what makes the argument valid even when the block $B$ is nonzero.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [9G](../../9g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
