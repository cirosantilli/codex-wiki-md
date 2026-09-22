<h1 id="p4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a QR factorization, whose existence is supplied. Since $|\det Q|=1$ and $R$ is triangular,

$$
|\det A|=|\det R|=\prod_{j=1}^n|r_{jj}|.
$$

Each diagonal entry is one component of its column, so $|r_{jj}|\leq\|r_j\|=\|a_j\|$. Multiplication yields [Hadamard determinant inequality](../../../../hadamard-determinant-inequality.md):

$$
\boxed{|\det A|\leq\prod_{j=1}^n\|a_j\|.}
$$

The argument includes singular matrices, since a zero diagonal factor makes the [determinant](../../../../determinant.md) zero.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [P4](../../p4.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
