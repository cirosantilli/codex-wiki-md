<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a_{ij}$ be the coefficient of $|ij\rangle$. The [partial trace](../../../../partial-trace.md) contracts the repeated index of the discarded [qubit](../../../../qubit.md):

$$
(\rho_1)_{ii'}=\sum_{j=0}^1a_{ij}\overline{a_{i'j}},
\qquad
(\rho_2)_{jj'}=\sum_{i=0}^1a_{ij}\overline{a_{ij'}}.
$$

For the first [qubit](../../../../qubit.md), each diagonal entry is $1/3+1/6=1/2$ and the upper off-diagonal entry is $1/3-1/6=1/6$. For the second [qubit](../../../../qubit.md), the diagonal entries are $2/3$ and $1/3$, while the upper off-diagonal entry is $-1/\sqrt{18}+1/\sqrt{18}=0$. Thus the two [reduced density matrices](../../../../reduced-density-matrix.md), each in [computational basis](../../../../computational-basis.md) order $0,1$, are

$$
\boxed{\rho_1=\operatorname{Tr}_2\rho=\begin{pmatrix}1/2&1/6\\1/6&1/2\end{pmatrix},\qquad
\rho_2=\operatorname{Tr}_1\rho=\begin{pmatrix}2/3&0\\0&1/3\end{pmatrix}.}
$$

Both have [eigenvalues](../../../../eigenvalue.md) $2/3,1/3$ and [trace](../../../../matrix-trace.md) one, so both are [mixed states](../../../../mixed-state.md) even though the joint [quantum state](../../../../quantum-state.md) is pure. Their different [eigenvectors](../../../../eigenvector.md) are visible in the useful rewrite

$$
|\psi\rangle=\sqrt{\frac23}|+\rangle|0\rangle-\sqrt{\frac13}|-\rangle|1\rangle,
\qquad |\pm\rangle=\frac{|0\rangle\pm|1\rangle}{\sqrt2}.
$$

Absorbing the minus sign into one local basis vector makes this a [Schmidt decomposition](../../../../schmidt-decomposition.md) with nonnegative coefficients. It also checks both [partial traces](../../../../partial-trace.md) and exhibits the [entanglement](../../../../entangled-state.md) responsible for the mixed local descriptions.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
