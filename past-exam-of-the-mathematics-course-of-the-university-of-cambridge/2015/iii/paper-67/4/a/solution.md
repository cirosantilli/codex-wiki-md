<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here is a finite-dimensional form of the [Kitaev geometrical lemma](../../../../../../kitaev-geometrical-lemma.md). Let $A,B$ be [positive operators](../../../../../../positive-operator.md), with nullspaces $S_A,S_B$ and all positive [eigenvalues](../../../../../../eigenvalue.md) at least $\gamma>0$. First assume $S_A\cap S_B=\{0\}$. Let $P,Q$ be the [orthogonal projections](../../../../../../orthogonal-projection.md) onto those nullspaces, and define their [smallest angle between two subspaces](../../../../../../smallest-angle-between-two-subspaces.md) by

$$
\cos\vartheta=
\sup_{\substack{u\in S_A,\ v\in S_B\\\|u\|=\|v\|=1}}
|\langle u,v\rangle|
=\|PQ\|,\qquad 0<\vartheta\leq\pi/2.
$$

If either nullspace is zero, set $\cos\vartheta=0$. Then

$$
\boxed{A+B\geq
\gamma(1-\cos\vartheta)I
=2\gamma\sin^2(\vartheta/2)I.}
$$

To prove it, spectral decomposition gives $A\geq\gamma(I-P)$ and $B\geq\gamma(I-Q)$. Write $C=P+Q$ and $c=\cos\vartheta$. For every vector $z$,

$$
\begin{aligned}
\langle z,C^2z\rangle
&=\|Pz\|^2+\|Qz\|^2+2\operatorname{Re}\langle Pz,Qz\rangle\\
&\leq\|Pz\|^2+\|Qz\|^2+2c\|Pz\|\|Qz\|\\
&\leq(1+c)(\|Pz\|^2+\|Qz\|^2)
=(1+c)\langle z,Cz\rangle.
\end{aligned}
$$

Thus $C^2\leq(1+c)C$. Since $C$ is [positive semidefinite](../../../../../../positive-semidefinite-matrix.md), each of its [eigenvalues](../../../../../../eigenvalue.md) lies in $[0,1+c]$, so $2I-C\geq(1-c)I$. Consequently

$$
A+B\geq\gamma(2I-P-Q)\geq\gamma(1-c)I,
$$

as claimed.

If there is a common nullspace $S=S_A\cap S_B$, restrict to $S^\perp$ and define the angle between $S_A\cap S^\perp$ and $S_B\cap S^\perp$ there. The same proof bounds the smallest positive [eigenvalue](../../../../../../eigenvalue.md) of $A+B$ by $2\gamma\sin^2(\vartheta/2)$, while $S$ is its zero-energy subspace. This version gives a [spectral gap](../../../../../../spectral-gap.md) above a possibly degenerate [ground state](../../../../../../ground-state.md) space.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
