<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

With no access to the discarded [qubit](../../../../qubit.md), the two preparations are exactly the [reduced density matrices](../../../../reduced-density-matrix.md) in [c](../c.md), with equal prior [probabilities](../../../../probability.md). Their difference is

$$
\Delta=\rho_1-\rho_2=\frac16\begin{pmatrix}-1&1\\1&1\end{pmatrix},
\qquad \Delta^2=\frac1{18}I.
$$

Since $\operatorname{Tr}\Delta=0$, its [eigenvalues](../../../../eigenvalue.md) are $\pm\sqrt2/6$. The [trace norm](../../../../trace-norm.md) and [trace distance](../../../../trace-distance.md) are consequently

$$
\|\Delta\|_{\rm tr}=\frac{\sqrt2}{3},
\qquad
\boxed{T(\rho_1,\rho_2)=\frac{\sqrt2}{6}.}
$$

The [Holevo–Helstrom theorem](../../../../holevo-helstrom-theorem.md) gives the optimum

$$
\boxed{P_{\rm success}^{\rm max}=\frac12\left(1+\frac{\sqrt2}{6}\right)
=\frac12+\frac{\sqrt2}{12}\simeq0.617851.}
$$

To establish attainability, rather than only an upper bound, measure the [Hermitian operator](../../../../hermitian-operator.md)

$$
B=\frac{X-Z}{\sqrt2},\qquad
X=\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix},
$$

where $X,Z$ are [Pauli matrices](../../../../pauli-matrices.md). Since $\Delta=(\sqrt2/6)B$, report **first qubit for the positive outcome; second qubit for the negative outcome**. The corresponding [orthogonal projections](../../../../orthogonal-projection.md) are $E_\pm=(I\pm B)/2$. Their success [probability](../../../../probability.md) is

$$
\frac12\operatorname{Tr}(E_+\rho_1)+\frac12\operatorname{Tr}(E_-\rho_2)
=\frac12+\frac12\operatorname{Tr}(E_+\Delta)
=\frac12+\frac{\sqrt2}{12},
$$

which reaches the bound. Identical [eigenvalues](../../../../eigenvalue.md) of the two [density matrices](../../../../density-matrix-split.md) do not make them indistinguishable: their eigenvectors differ, and this [quantum measurement](../../../../quantum-measurement-split.md) detects that difference.

## ↑ Ancestors (12)

1. [E](../e.md)
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
