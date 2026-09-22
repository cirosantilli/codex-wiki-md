<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a spatial [discrete Fourier mode](../../../../../../discrete-fourier-mode.md) $u_{k,j}^n=a_ne^{i(k\xi+j\eta)}$. Its recurrence and [amplification polynomial of a multilevel finite difference scheme](../../../../../../amplification-polynomial-of-a-multilevel-finite-difference-scheme.md) are

$$
a_{n+1}=2is\,a_n+a_{n-1},\qquad G^2-2isG-1=0,\qquad
s=\mu(\sin\xi+\sin\eta).
$$

The [polynomial roots](../../../../../../root-of-a-polynomial.md) are $G_\pm=is\pm\sqrt{1-s^2}$. For $|s|<1$ both have modulus one and are separated. Since $|\sin\xi+\sin\eta|\le2$, a fixed $0<\mu<1/2$ bounds their separation below by $2\sqrt{1-4\mu^2}$. The two-level [companion matrix](../../../../../../companion-matrix.md) is therefore diagonalizable with uniformly bounded [eigenvector](../../../../../../eigenvector.md) [matrix](../../../../../../matrix.md) and inverse. To see the uniform bound explicitly, write $V=\begin{pmatrix}G_+&G_-\\1&1\end{pmatrix}$. Its determinant is $G_+-G_-$; all its entries have modulus one, and those of $V^{-1}$ are bounded by the reciprocal of the root separation. The companion matrix powers are $V\operatorname{diag}(G_+^n,G_-^n)V^{-1}$, bounded independently of frequency and step number. [Parseval's identity](../../../../../../parseval-identity.md) converts this into a mesh-independent discrete $L^2$ bound for arbitrary perturbations at the two initial levels.

If $\mu>1/2$, choose $\xi=\eta=\pi/2$. Then $s=2\mu>1$, and one [polynomial root](../../../../../../root-of-a-polynomial.md) has modulus $s+\sqrt{s^2-1}>1$. On periodic meshes with the number of points divisible by four, this is an actual grid mode, producing exponential [linear instability](../../../../../../linear-instability.md).

At $\mu=1/2$ the same phases give $(G-i)^2$. The [companion matrix](../../../../../../companion-matrix.md) is not a [scalar matrix](../../../../../../scalar-matrix.md), so the double [polynomial root](../../../../../../root-of-a-polynomial.md) has a nontrivial [Jordan block](../../../../../../jordan-block.md). The solution $a_n=ni^n$ has bounded starting amplitudes but grows like $n$. On a fixed physical time interval $n$ is of order $1/k$, so no mesh-independent [stability](../../../../../../stability-of-a-numerical-method.md) bound exists. Consequently

$$
\boxed{0<\mu<\tfrac12}
$$

is the [stability](../../../../../../stability-of-a-numerical-method.md) interval under the standard two-level definition. Testing only [polynomial root](../../../../../../root-of-a-polynomial.md) moduli would misleadingly include the endpoint. A special startup selecting the non-growing branch at that endpoint restricts the perturbations and does not establish [stability](../../../../../../stability-of-a-numerical-method.md) of the full recurrence. This is the [two-dimensional leapfrog stability threshold](../../../../../../two-dimensional-leapfrog-stability-threshold.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
