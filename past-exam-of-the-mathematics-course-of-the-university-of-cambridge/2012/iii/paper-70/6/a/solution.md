<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [orthonormal](../../../../../../orthonormal-set.md) [multiresolution analysis](../../../../../../multiresolution-analysis.md) consists of [closed subspaces of a Hilbert space](../../../../../../closed-subspace-of-a-hilbert-space.md) $(V_j)_{j\in\mathbb Z}$ of the [Hilbert space](../../../../../../hilbert-space-split.md) $L^2(\mathbb R)$ such that

$$
V_j\subset V_{j+1},\qquad\overline{\bigcup_jV_j}=L^2(\mathbb R),\qquad\bigcap_jV_j=\{0\},\qquad
g\in V_j\ \Longleftrightarrow\ g(2\cdot)\in V_{j+1}.
$$

There is a [scaling function](../../../../../../scaling-function.md) $\phi$ whose [integer](../../../../../../integer.md) [function translations](../../../../../../translation-of-a-function.md) form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $V_0$. Consequently $\phi_{j,k}(x)=2^{j/2}\phi(2^jx-k)$ form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $V_j$; in particular $V_0$ is invariant under [integer](../../../../../../integer.md) [function translations](../../../../../../translation-of-a-function.md).

Let $W_j=V_{j+1}\ominus V_j$ be the [orthogonal complement](../../../../../../orthogonal-complement.md) of $V_j$ in $V_{j+1}$. Nesting, density and the trivial intersection imply the [orthogonal direct sum](../../../../../../orthogonal-direct-sum.md)

$$
L^2(\mathbb R)=\bigoplus_{j\in\mathbb Z}W_j.
$$

For example, telescoping $V_{J+1}=V_L\oplus\bigoplus_{j=L}^JW_j$ and letting $L\to-\infty$, $J\to\infty$ gives this decomposition; the corresponding [orthogonal projections](../../../../../../orthogonal-projection.md) converge strongly to zero and the identity by the intersection and density properties.

To construct the [orthonormal wavelet](../../../../../../orthonormal-wavelet.md), use $\phi\in V_1$ to write the [scaling refinement equation](../../../../../../scaling-refinement-equation.md) $\phi=\sum_na_n\phi(2\cdot-n)$, with $a\in\ell^2$ and $\sum_n|a_n|^2=2$. Put $m(t)=\frac12\sum_na_ne^{-int}$. The [orthonormal translates and Fourier periodization](../../../../../../orthonormal-translates-and-fourier-periodization.md) criterion proved in part (b), applied to the [scaling refinement equation](../../../../../../scaling-refinement-equation.md), yields

$$
1=\sum_k|\widehat\phi(2t+2\pi k)|^2
=|m(t)|^2\sum_\ell|\widehat\phi(t+2\pi\ell)|^2+|m(t+\pi)|^2\sum_\ell|\widehat\phi(t+\pi+2\pi\ell)|^2
=|m(t)|^2+|m(t+\pi)|^2.
$$

This is the [quadrature mirror filter](../../../../../../quadrature-mirror-filter.md) identity. Define

$$
q(t)=-e^{-it}\overline{m(t+\pi)},\qquad b_n=(-1)^n\overline{a_{1-n}},\qquad
\psi(x)=\sum_nb_n\phi(2x-n).
$$

The [Fourier series](../../../../../../fourier-series-split.md) of $q$ is $\frac12\sum_nb_ne^{-int}$, and $\widehat\psi(2t)=q(t)\widehat\phi(t)$. The two rows $(m(t),m(t+\pi))$ and $(q(t),q(t+\pi))$ form a unitary $2\times2$ [matrix](../../../../../../matrix.md) almost everywhere: both have squared [norm](../../../../../../norm.md) one and their [inner product](../../../../../../inner-product.md) is zero. This [wavelet completion of a multiresolution filter](../../../../../../wavelet-completion-of-a-multiresolution-filter.md) proves not just orthogonality but completeness. Splitting a finer-scale coefficient [Fourier series](../../../../../../fourier-series-split.md) into its values at $t$ and $t+\pi$, this invertible two-channel matrix resolves it into a coarse-scale channel and its complementary channel. Thus the [integer](../../../../../../integer.md) [function translations](../../../../../../translation-of-a-function.md) of $\psi$ form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $W_0$.

The dilated [functions](../../../../../../function-split.md) $\psi_{j,k}(x)=2^{j/2}\psi(2^jx-k)$ therefore form an [orthonormal basis](../../../../../../orthonormal-basis.md) of each $W_j$. The [orthogonal direct sum](../../../../../../orthogonal-direct-sum.md) proves the conclusion: **every [orthonormal](../../../../../../orthonormal-set.md) multiresolution analysis produces an [orthonormal](../../../../../../orthonormal-set.md) wavelet [basis](../../../../../../basis.md)** $\{\psi_{j,k}:j,k\in\mathbb Z\}$ of $L^2(\mathbb R)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
