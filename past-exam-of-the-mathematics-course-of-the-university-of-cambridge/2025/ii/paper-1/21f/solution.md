<h1 id="21f/solution">Solution</h1>

↑ **Parent:** [21F](../21f.md)

The simplicial [Mayer–Vietoris theorem](../../../../../mayer-vietoris-sequence.md) says that if a simplicial complex $X=M\cup N$ for subcomplexes $M,N$, there is a natural long exact [sequence](../../../../../sequence.md)

$$
\cdots\to H_n(M\cap N)\xrightarrow{(i_*,-j_*)}
H_n(M)\oplus H_n(N)\to H_n(X)\to H_{n-1}(M\cap N)\to\cdots.
$$

The reduced version extends through dimension zero.

For every simplex $\sigma$ of $K$, all faces of $\sigma\cup\{c_i\}$ are either faces of $\sigma$ or have the form $\tau\cup\{c_i\}$ with $\tau$ a face of $\sigma$, so they lie in $L$. Each $c_i*K$ is a cone and hence a simplicial complex. For distinct $i,j$, the rays in the last two coordinates through $c_i$ and $c_j$ are not positive multiples. Thus the two cones meet exactly in $K$, so their simplices have common faces only in $K$. Hence $L$ is a simplicial complex.

Topologically, $L$ is the union of three cones on $K$ along their common base. The first two cones form the suspension $\Sigma K$. Attaching the third contractible cone along the equatorial copy of $K$ gives

$$
L\simeq\Sigma K\vee\Sigma K.
$$

This also follows by applying reduced Mayer--Vietoris twice: every cone has zero reduced homology, and the two inclusion maps from the common base are null-homotopic inside the cones. Therefore

$$
\boxed{\widetilde H_n(L)\cong
\widetilde H_{n-1}(K)\oplus\widetilde H_{n-1}(K)}
$$

for every $n$, with the convention that negative reduced homology vanishes. Since $K$ is nonempty, $L$ is connected, so explicitly

$$
H_0(L)\cong\mathbb Z,\qquad
H_1(L)\cong\widetilde H_0(K)^{\oplus2},
$$



$$
H_n(L)\cong H_{n-1}(K)^{\oplus2}\quad(n\geq2).
$$

## ↑ Ancestors (10)

1. [21F](../21f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
