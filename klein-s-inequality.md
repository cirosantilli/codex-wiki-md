<h1 id="klein-s-inequality">Klein's inequality</h1>

↑ **Parent:** [Matrix logarithm](matrix-logarithm.md)

For positive-definite [Hermitian matrices](hermitian-operator.md) $A,B$, Klein's inequality gives

$$
\operatorname{Tr}[A(\ln A-\ln B)]\geq\operatorname{Tr}(A-B),
$$

with equality exactly when $A=B$. To prove it, let $a_i,b_j$ be their [eigenvalues](eigenvalue.md) and $u_i,v_j$ their orthonormal eigenvectors. The weights $w_{ij}=|\langle u_i,v_j\rangle|^2$ have row and column sums one. The difference between the two sides is

$$
\sum_{i,j}w_{ij}\left[a_i\ln\frac{a_i}{b_j}-a_i+b_j\right]\geq0
$$

by the scalar [logarithm inequality](logarithm-inequality.md) $\ln t\leq t-1$. Equality requires $a_i=b_j$ whenever $w_{ij}>0$, implying $A=B$. Limits extend the result to positive semidefinite matrices with the appropriate support condition. Applying it to trace-one matrices proves [nonnegativity of quantum relative entropy](nonnegativity-of-quantum-relative-entropy.md).

## ↑ Ancestors (9)

1. [Matrix logarithm](matrix-logarithm.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Nonnegativity of quantum relative entropy](nonnegativity-of-quantum-relative-entropy.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/5/ii/solution.md)
- [Relative-entropy identity for rank-one dephasing](relative-entropy-identity-for-rank-one-dephasing.md)
