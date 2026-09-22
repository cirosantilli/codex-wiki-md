<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The commuting terms

$$
S_j=X_jX_{j+1},\qquad 1\leq j<n,
$$

are independent [stabilizer generators](../../../../../../stabilizer-group.md). Since $J>0$, every ground state has $S_j=+1$. The resulting two-dimensional [stabilizer subspace](../../../../../../stabilizer-subspace.md) is

$$
\mathcal C_n^Z=\operatorname{span}\{|+\rangle^{\otimes n},|-\rangle^{\otimes n}\},
$$

the [phase-flip repetition code](../../../../../../phase-flip-repetition-code.md). A convenient pair of logical Pauli operators is

$$
\overline Z=X_1,
\qquad
\overline X=Z_1Z_2\cdots Z_n.
$$

Indeed, they commute with every stabilizer, anticommute with each other, and are not stabilizers.

For phase-flip errors $E_A=\prod_{j\in A}Z_j$ and $E_B=\prod_{j\in B}Z_j$, the operator entering the [Knill--Laflamme condition](../../../../../../knill-laflamme-condition.md) is $E_A^\dagger E_B=E_{A\triangle B}$ and has weight at most $2t$. Every nonempty proper product of $Z_j$ anticommutes with some $S_j$ unless it is the full logical operator $\overline X$. The Knill--Laflamme conditions therefore hold whenever $2t<n$, and fail once two allowed errors can differ by $\overline X$. Thus

$$
\boxed{t=\left\lfloor\frac{n-1}{2}\right\rfloor.}
$$

Each physical $X_j$ commutes with all stabilizers, and $X_jX_1$ is a product of stabilizers. Hence every $X_j$ acts on the code as the undetectable logical operator $\overline Z$. The code cannot detect, and therefore cannot correct, even a single bit flip.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
