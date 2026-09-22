<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An orthonormal [multiresolution analysis](../../../../../../multiresolution-analysis.md) consists of closed subspaces $V_j\subset L_2(\mathbb R)$, $j\in\mathbb Z$, with $V_j\subset V_{j+1}$, $\overline{\bigcup_jV_j}=L_2(\mathbb R)$, $\bigcap_jV_j=\{0\}$, and the dilation equivalence $h\in V_j\iff h(2\cdot)\in V_{j+1}$. A [scaling function](../../../../../../scaling-function.md) $\phi$ has integer translates forming an [orthonormal basis](../../../../../../orthonormal-basis.md) of $V_0$. Hence

$$
\phi_{j,k}(x)=2^{j/2}\phi(2^jx-k),\qquad k\in\mathbb Z,
$$

is an [orthonormal basis](../../../../../../orthonormal-basis.md) of $V_j$. Set $W_j=V_{j+1}\ominus V_j$, the [orthogonal complement](../../../../../../orthogonal-complement.md) of $V_j$ inside $V_{j+1}$. A function $\psi$ whose integer translates form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $W_0$ produces a complete [orthonormal wavelet](../../../../../../orthonormal-wavelet.md) system $\{2^{j/2}\psi(2^j\cdot-k):j,k\in\mathbb Z\}$: different $W_j$ are orthogonal, their sum contains every difference $V_b\ominus V_a$, and density together with the zero intersection exhausts $L_2(\mathbb R)$.

Here is the filter construction that guarantees such a [wavelet](../../../../../../wavelet.md). Nesting puts $\phi$ in $V_1$, so expansion in its [orthonormal basis](../../../../../../orthonormal-basis.md) gives the [scaling refinement equation](../../../../../../scaling-refinement-equation.md) $\phi=\sum_na_n\phi(2\cdot-n)$, with $a\in\ell_2$. Define the [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) and its complementary [quadrature mirror filter](../../../../../../quadrature-mirror-filter.md) by

$$
m(t)=\tfrac12\sum_na_ne^{-int},\qquad q(t)=-e^{-it}\overline{m(t+\pi)}.
$$

Splitting the [orthonormal translates and Fourier periodization](../../../../../../orthonormal-translates-and-fourier-periodization.md) identity at $2t$, as in part (b), gives $|m(t)|^2+|m(t+\pi)|^2=1$ almost everywhere. Consequently the rows of

$$
\begin{pmatrix}m(t)&m(t+\pi)\\-e^{-it}\overline{m(t+\pi)}&e^{-it}\overline{m(t)}\end{pmatrix}
$$

have length one and are orthogonal; the matrix is unitary. Put $b_n=(-1)^n\overline{a_{1-n}}$ and $\psi=\sum_nb_n\phi(2\cdot-n)$, so $q(t)=\tfrac12\sum_nb_ne^{-int}$.

To see completeness as well as orthogonality, identify $V_1$ with its fine-scale coefficient sequences and take their [Fourier series](../../../../../../fourier-series-split.md). Group the frequencies $t$ and $t+\pi$ over a half-period. The two rows of the displayed matrix are the normalized coarse and complementary channels; their unitarity is exactly an onto isometry from these two channels to the fine-scale coefficient space. Translates of $\phi$ and $\psi$ correspond to the [Fourier basis](../../../../../../fourier-basis.md) in the respective channels. They therefore jointly form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $V_1$. The [orthogonal complement](../../../../../../orthogonal-complement.md) channel gives the [wavelet completion of a multiresolution filter](../../../../../../wavelet-completion-of-a-multiresolution-filter.md), namely the integer translates of $\psi$ span $W_0$. This proves the asserted relation with an [orthonormal wavelet](../../../../../../orthonormal-wavelet.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
