<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md), $\Delta=-\operatorname{div}\nabla$. A [flat torus](../../../../../flat-torus.md) is the quotient $\mathbb R^d/\Lambda$, where $\Lambda$ is a full-rank [Euclidean lattice](../../../../../euclidean-lattice.md) and the metric descends from the [Euclidean metric](../../../../../euclidean-metric.md). Its [dual lattice](../../../../../dual-lattice.md) is

$$
\Lambda^*=\{\xi\in\mathbb R^d:\langle\xi,\ell\rangle\in\mathbb Z\text{ for every }\ell\in\Lambda\}.
$$

If $V$ is the [covolume](../../../../../covolume.md) of $\Lambda$, the functions $\phi_\xi(x)=V^{-1/2}e^{2\pi i\langle\xi,x\rangle}$ descend to the torus. Direct differentiation gives the [spectrum of a flat torus](../../../../../spectrum-of-a-flat-torus.md):

$$
\boxed{\Delta\phi_\xi=4\pi^2|\xi|^2\phi_\xi,\qquad
\operatorname{Spec}\Delta=\{4\pi^2|\xi|^2:\xi\in\Lambda^*\}.}
$$

The multiset includes one entry for each dual vector. In particular zero has multiplicity one. Writing $\Lambda=B\mathbb Z^d$ identifies the dual vectors with $B^{-T}m$, $m\in\mathbb Z^d$. Standard [Fourier series](../../../../../fourier-series-split.md) on the unit cube then prove that these functions are an [orthonormal basis](../../../../../orthonormal-basis.md) of $L^2$ on the torus. If $\Delta f=\lambda f$, its [Fourier coefficients](../../../../../fourier-coefficient.md) satisfy $(4\pi^2|\xi|^2-\lambda)\widehat f(\xi)=0$. Thus every [eigenfunction](../../../../../eigenfunction.md) is a linear combination of the indicated shell of frequencies, with no additional [eigenvalues](../../../../../eigenvalue.md). Compactness gives the discrete self-adjoint realization, whose [eigenfunctions](../../../../../eigenfunction.md) are smooth. For real functions the two characters at $\xi,-\xi$ become cosine and sine, giving the same real multiplicities. The opposite Laplacian sign would negate all displayed [eigenvalues](../../../../../eigenvalue.md) without changing the rigidity conclusion.

To prove two-dimensional [spectral rigidity](../../../../../spectral-rigidity.md), let $L=\Lambda^*$ and recover its [Gram matrix](../../../../../gram-matrix.md) from its vector-length multiset. Let $a$ be the shortest nonzero length and choose $v\in L$ with $|v|=a$. This vector is primitive: a proper integer multiple would have a shorter lattice vector. Hence $L\cap\mathbb Rv=\mathbb Zv$. From the spectral multiset subtract exactly two occurrences of each length $ka$, $k=1,2,\ldots$. The remaining multiset consists precisely of the vectors not on this line, including correct multiplicities at coincident lengths. Its least length $b$ is the length of a shortest vector $w$ independent of $v$.

The pair $(v,w)$ is a [basis](../../../../../basis.md) of $L$. Otherwise take a lattice point in a nonzero coset of $\mathbb Zv+\mathbb Zw$ and reduce its two coefficients into $[-1/2,1/2]$. The resulting nonzero lattice vector $z=\alpha v+\beta w$ is not on $\mathbb Rv$, by primitivity of $v$. But

$$
|z|\leq\frac{|v|+|w|}{2}\leq b,
$$

with strict inequality: when both coefficients are nonzero the triangle inequality is strict for independent vectors, and when one vanishes its length is at most $b/2$. This contradicts the definition of $b$. Subtract an integer multiple of $v$ from $w$ and, if necessary, change its sign to arrange $0\leq c=\langle v,w\rangle\leq a^2/2$; minimality of $b$ makes this reduction possible without decreasing its length.

The [covolume](../../../../../covolume.md) $A$ of $L$ is also spectral. The count of lattice vectors with length at most $R$ obeys

$$
\#(L\cap B_R)=\frac{\pi R^2}{A}+O(R).
$$

For example, translate a bounded fundamental parallelogram of diameter bound $D$: the union of tiles with centres in $B_R$ contains $B_{R-D}$ and lies inside $B_{R+D}$. Comparing their areas proves the leading coefficient. The [spectrum](../../../../../spectrum-functional-analysis.md) supplies this count. Since $(v,w)$ is a lattice [basis](../../../../../basis.md), its parallelogram area satisfies $A^2=a^2b^2-c^2$. Therefore

$$
\boxed{\operatorname{Gram}(v,w)=
\begin{pmatrix}a^2&\sqrt{a^2b^2-A^2}\\\sqrt{a^2b^2-A^2}&b^2\end{pmatrix}.}
$$

All three quantities are determined by the [spectrum](../../../../../spectrum-functional-analysis.md). Equal [Gram matrices](../../../../../gram-matrix.md) give an orthogonal map between the [dual lattices](../../../../../dual-lattice.md); taking duals gives an orthogonal map between the original lattices, descending to a [Riemannian isometry](../../../../../riemannian-isometry.md) of the tori. **Isospectral flat two-tori are isometric.** This is the [two-dimensional lattice reconstruction from vector lengths](../../../../../two-dimensional-lattice-reconstruction-from-vector-lengths.md); it uses lengths with multiplicities, not merely the set of distinct lengths.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
