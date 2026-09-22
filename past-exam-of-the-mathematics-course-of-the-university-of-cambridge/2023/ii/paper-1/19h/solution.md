<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

A [complex representation](../../../../../complex-representation.md) of a finite group $G$ is a homomorphism

$$
\rho:G\longrightarrow\operatorname{GL}(V)
$$

for a finite-dimensional complex vector space $V$. It is an [irreducible representation](../../../../../irreducible-representation.md) when its only invariant subspaces are $0$ and $V$, and its [degree](../../../../../degree-of-a-representation.md) is $\dim V$. Two representations are [isomorphic](../../../../../isomorphic-representations.md) when there is an invertible linear map intertwining their $G$-actions.

Write the [dihedral group](../../../../../dihedral-group.md) as

$$
D_{2n}=\langle r,s:r^n=s^2=1,\ srs=r^{-1}\rangle.
$$

In an irreducible representation choose an [eigenvector](../../../../../eigenvector.md) $0\ne v\in V$ of $\rho(r)$, which is possible because $r^n=1$. If its [eigenvalue](../../../../../eigenvalue.md) is $\lambda$, then

$$
\rho(r)\rho(s)v
=\rho(s)\rho(r)^{-1}v
=\lambda^{-1}\rho(s)v.
$$

Thus $W=\operatorname{span}\{v,\rho(s)v\}$ is invariant under both $r$ and $s$. Irreducibility forces $W=V$, proving $\dim V\leq2$ as in [irreducible complex representations of a finite dihedral group](../../../../../irreducible-complex-representations-of-a-finite-dihedral-group.md).

Let $\omega=e^{2\pi i/n}$. Besides the one-dimensional representations described below, define for each indicated $j$

$$
\rho_j(r)=
\begin{pmatrix}\omega^j&0\\0&\omega^{-j}\end{pmatrix},
\qquad
\rho_j(s)=
\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

These matrices satisfy the defining relations. Since $\omega^j\ne\omega^{-j}$, the only one-dimensional $r$-invariant subspaces are the two coordinate axes, and $s$ interchanges them. Hence $\rho_j$ is irreducible. Their [characters](../../../../../character-of-a-representation.md) satisfy

$$
\chi_j(r)=2\cos\frac{2\pi j}{n},
$$

whose values are distinct in the ranges below, so the $\rho_j$ are pairwise nonisomorphic. This is the family of [two-dimensional representations of a finite dihedral group](../../../../../two-dimensional-representations-of-a-finite-dihedral-group.md).

If $n$ is odd, a [one-dimensional character](../../../../../one-dimensional-character.md) must send $r$ to a scalar $\varepsilon$ satisfying $\varepsilon^n=1$ and $\varepsilon=\varepsilon^{-1}$. Thus $\varepsilon=1$, while $s$ may independently map to $1$ or $-1$. These give two one-dimensional irreducibles. Taking

$$
j=1,\ldots,\frac{n-1}{2}
$$

gives $(n-1)/2$ two-dimensional irreducibles, for a total of

$$
2+\frac{n-1}{2}=\frac{n+3}{2}.
$$

If $n$ is even, $r$ may map to either $1$ or $-1$, and again $s$ may map independently to either sign. This gives four pairwise nonisomorphic one-dimensional irreducibles. Taking

$$
j=1,\ldots,\frac n2-1
$$

gives $n/2-1$ two-dimensional irreducibles, for a total of

$$
4+\left(\frac n2-1\right)=\frac{n+6}{2}.
$$

Different dimensions distinguish the one- and two-dimensional families, completing the required construction and justification.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
