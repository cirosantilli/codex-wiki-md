<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

In the history basis, $M(s)=(1-s)D+sE$ is a Hermitian tridiagonal matrix. Its first diagonal entry is $s/2$, its interior entries are $1$, its last entry is $1-s/2$, and each off-diagonal entry is $-s/2$.

The [Gershgorin disc theorem](../../../../../../../gershgorin-circle-theorem.md) confines the first row's [eigenvalue](../../../../../../../eigenvalue.md) to $[0,s]$, the interior rows to $[1-s,1+s]$, and the last row to $[1-s,1]$. For $0\leq s\leq1/3$, the first disc is disjoint from all the others and therefore contains exactly one [eigenvalue](../../../../../../../eigenvalue.md). Since $M(s)$ is [positive semidefinite](../../../../../../../positive-semidefinite-matrix.md), that eigenvalue is the [ground state](../../../../../../../ground-state.md) energy. All other [eigenvalues](../../../../../../../eigenvalue.md) are at least $1-s$, while the lowest is at most $s$. Hence the [Gershgorin gap bound for an adiabatic history path](../../../../../../../gershgorin-gap-bound-for-an-adiabatic-history-path.md) gives

$$
\boxed{\Delta(M(s))\geq1-2s\geq\frac13
\qquad(0\leq s\leq1/3).}
$$

This argument also covers $s=0$, where the first disc is the isolated point zero.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 67](../../../../paper-67-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
