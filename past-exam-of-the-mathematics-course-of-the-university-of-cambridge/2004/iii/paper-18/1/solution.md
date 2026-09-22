<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $M=\mathbb R^d/\Lambda$ be a [flat torus](../../../../../flat-torus.md), where $\Lambda$ is a full-rank [Euclidean lattice](../../../../../euclidean-lattice.md), and use the nonnegative [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) $\Delta=-\sum_{k=1}^d\partial_k^2$. The [dual lattice](../../../../../dual-lattice.md) is

$$
\Lambda^*=\{w\in\mathbb R^d:\langle w,v\rangle\in\mathbb Z\text{ for every }v\in\Lambda\}.
$$

For $w\in\Lambda^*$, the function $\phi_w(x)=\operatorname{vol}(M)^{-1/2}e^{2\pi i\langle w,x\rangle}$ is periodic under $\Lambda$, so it defines a function on $M$, and direct differentiation gives $\Delta\phi_w=4\pi^2|w|^2\phi_w$. Integrating characters on a fundamental parallelepiped proves that these functions are orthonormal. After choosing a lattice basis, the ordinary [Fourier series](../../../../../fourier-series-split.md) theorem on $\mathbb R^d/\mathbb Z^d$ proves completeness, so there are no additional [eigenvalues](../../../../../eigenvalue.md). Thus the [spectrum of a flat torus](../../../../../spectrum-of-a-flat-torus.md) is

$$
\boxed{\operatorname{Spec}(\Delta_M)=\{4\pi^2|w|^2:w\in\Lambda^*\},}
$$

with multiplicity equal to the number of dual vectors of the given length; the zero [eigenvalue](../../../../../eigenvalue.md) occurs once.

It remains to show that a two-dimensional [Euclidean lattice](../../../../../euclidean-lattice.md) is determined up to an orthogonal transformation by its vector-length multiset. This is the [two-dimensional lattice reconstruction from vector lengths](../../../../../two-dimensional-lattice-reconstruction-from-vector-lengths.md). Let $v$ be a shortest nonzero vector, of length $a$. It is primitive: $v=ku$ with integer $|k|>1$ would give a shorter nonzero vector. The lattice vectors on its line are therefore precisely the integer multiples of $v$. Subtract two occurrences of each length $ka$, $k=1,2,\ldots$, from the length multiset. This removes exactly one primitive lattice line, even when other vectors happen to have the same lengths. The smallest remaining length $b$ is the length of a shortest vector $w$ independent of $v$.

These two vectors form a [basis](../../../../../basis.md) of the lattice. Otherwise a nonzero coset of $\mathbb Zv+\mathbb Zw$ has a lattice representative $u=sv+tw$ with $|s|,|t|\leq1/2$. It cannot have $t=0$, since primitivity of $v$ would then force $u=0$. It is therefore independent of $v$, while

$$
|u|\leq|s|a+|t|b\leq\tfrac12(a+b)\leq b.
$$

The inequality is strict: if both coefficients are nonzero, the vectors are not parallel and the triangle inequality is strict; if $s=0$, then $|u|\leq b/2$. This contradicts the choice of $w$.

The [covolume](../../../../../covolume.md) $A$ is also determined by the length multiset. If $N(R)$ counts lattice vectors in a radius-$R$ disk, then

$$
N(R)=\frac{\pi R^2}{A}+O(R),\qquad A=\lim_{R\to\infty}\frac{\pi R^2}{N(R)}.
$$

To justify the estimate, tile the plane by a bounded fundamental parallelogram. Only cells meeting a fixed-width neighbourhood of the disk boundary contribute an error; their total number is $O(R)$. The lattice basis $v,w$ has [Gram matrix](../../../../../gram-matrix.md)

$$
\begin{pmatrix}a^2&c\\c&b^2\end{pmatrix},\qquad a^2b^2-c^2=A^2.
$$

Thus $|c|=\sqrt{a^2b^2-A^2}$ is determined. Replacing $w$ by $-w$ makes $c\geq0$, so the [Gram matrix](../../../../../gram-matrix.md) is determined entirely. Equal [Gram matrices](../../../../../gram-matrix.md) give an orthogonal map between the lattice bases and hence between the lattices.

Two isospectral two-dimensional [flat tori](../../../../../flat-torus.md) consequently have orthogonally equivalent [dual lattices](../../../../../dual-lattice.md). Taking duals shows that their original lattices are orthogonally equivalent too, and the orthogonal map descends to an [isometry](../../../../../isometry.md) of the quotient tori. **Two isospectral flat tori of dimension two are isometric.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
