<h1 id="11/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If $K^2\ne W$, the three [eigenvalues](../../../../eigenvalue.md) are distinct, so a basis of [eigenvectors](../../../../eigenvector.md) gives

$$
\boxed{M'=\operatorname{diag}(-\rho_1,-\rho_2,0),\qquad
\rho_1=-K-\sqrt{K^2-W},\quad\rho_2=-K+\sqrt{K^2-W}.}
$$

The transformed coordinates then have the displayed exponential form. If $K^2<W$, this is a complex [eigenbasis](../../../../eigenbasis.md); real concentrations are recovered by conjugate-paired coefficients. A real basis instead gives a decaying two-dimensional rotation block with decay rate $-K$ and angular frequency $\sqrt{W-K^2}$.

The proposed [diagonalization](../../../../diagonalization-of-a-matrix.md) is **not valid for every positive choice of rates**. For example $\epsilon=\delta=1$, $\eta=4$ gives $K=-3$, $W=9$, with repeated [eigenvalue](../../../../eigenvalue.md) $-3$ and only one corresponding [eigenvector](../../../../eigenvector.md). More generally the [defective repeated eigenvalue in a cyclic conversion model](../../../../defective-repeated-eigenvalue-in-a-cyclic-conversion-model.md) occurs when $K^2=W$. A [Jordan basis](../../../../jordan-basis.md) then gives

$$
M'=\begin{pmatrix}K&1&0\\0&K&0\\0&0&0\end{pmatrix},\qquad
x'(t)=\begin{pmatrix}(c_1+c_2t)e^{Kt}\\c_2e^{Kt}\\c_3\end{pmatrix}.
$$

The extra factor $t$ cannot be represented by two independent pure exponential coordinates in a diagonal basis.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [11](../../11.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
