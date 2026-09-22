<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An orthonormal [multiresolution analysis](../../../../../../multiresolution-analysis.md) consists of closed subspaces $(V_j)_{j\in\mathbb Z}$ of the [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) $L^2(\mathbb R)$ with $V_j\subset V_{j+1}$, dense union, intersection $\{0\}$, and the dilation rule $f\in V_j\iff f(2\cdot)\in V_{j+1}$. A [scaling function](../../../../../../scaling-function.md) $\phi$ has integer translates forming an [orthonormal basis](../../../../../../orthonormal-basis.md) of $V_0$. Equivalently,

$$
\phi_{j,n}(x)=2^{j/2}\phi(2^jx-n),\qquad n\in\mathbb Z,
$$

form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $V_j$. Let $W_j=V_{j+1}\ominus V_j$. Density and the trivial intersection imply $L^2(\mathbb R)=\bigoplus_{j\in\mathbb Z}W_j$.

Nesting gives the [scaling refinement equation](../../../../../../scaling-refinement-equation.md) $\phi(x)=\sum_na_n\phi(2x-n)$, with $h_n=a_n/\sqrt2$ the coefficients in the normalized finer-scale basis. [Orthogonality](../../../../../../orthogonal-vectors.md) of the translates gives $\sum_na_n\overline{a_{n-2r}}=2\delta_{r0}$. Its Fourier form is the [quadrature mirror filter](../../../../../../quadrature-mirror-filter.md) identity $|m(t)|^2+|m(t+\pi)|^2=1$, where $m(t)=\tfrac12\sum_na_ne^{-int}$.

Set $b_n=(-1)^n\overline{a_{1-n}}$ and define $\psi(x)=\sum_nb_n\phi(2x-n)$ in $L^2$. Its high-pass symbol is $q(t)=-e^{-it}\overline{m(t+\pi)}$. The matrix

$$
\begin{pmatrix}m(t)&m(t+\pi)\\q(t)&q(t+\pi)\end{pmatrix}
$$

is unitary almost everywhere. Under the identification of $V_1$ with its finer-scale coefficient space, this two-channel unitary transform splits that space into the translates of $\phi$ and the translates of $\psi$. The latter are therefore an [orthonormal basis](../../../../../../orthonormal-basis.md) of $W_0$. Dilating gives **an [orthonormal wavelet](../../../../../../orthonormal-wavelet.md) basis**

$$
\boxed{\{2^{j/2}\psi(2^jx-n):j,n\in\mathbb Z\}\text{ of }L^2(\mathbb R).}
$$

This [wavelet completion of a multiresolution filter](../../../../../../wavelet-completion-of-a-multiresolution-filter.md) explains how the [multiresolution analysis](../../../../../../multiresolution-analysis.md) supplies a single [orthonormal wavelet](../../../../../../orthonormal-wavelet.md). The argument uses coefficient-space completeness, not just pairwise [orthogonality](../../../../../../orthogonal-vectors.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
