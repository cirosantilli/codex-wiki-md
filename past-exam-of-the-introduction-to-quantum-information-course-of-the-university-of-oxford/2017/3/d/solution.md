<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [universal NOT gate](../../../../universal-not-gate.md) is the [isotropic qubit map](../../../../isotropic-qubit-map.md) with factor $-1$. It sends

$$
\varrho=\frac12(I+\mathbf s\cdot\boldsymbol\sigma)
\quad\longmapsto\quad
\mathcal N(\varrho)=\frac12(I-\mathbf s\cdot\boldsymbol\sigma)=I-\varrho.
$$

For $|\mathbf s|\leq1$, the output has the same two nonnegative [eigenvalues](../../../../eigenvalue.md) as the input, exchanged, and still has [trace](../../../../matrix-trace.md) one. Thus **it maps every single-qubit density matrix to a density matrix**. Its linear extension to all operators is $\mathcal N(A)=\operatorname{tr}(A)I-A$, not $I-A$ for arbitrary unnormalized $A$. Positivity on one [qubit](../../../../qubit.md) does not establish [complete positivity](../../../../completely-positive-map.md) when an [ancilla](../../../../quantum-ancilla.md) is present.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
