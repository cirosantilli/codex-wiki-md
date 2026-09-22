<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an open subdomain $U\subset D$, identify $H_0^1(U)$ with the closed subspace of $H_0^1(D)$ obtained by zero extension. Its orthogonal complement is

$$
\mathcal H_U
=\{f\in H_0^1(D):(f,g)_\nabla=0
\text{ for every }g\in H_0^1(U)\}.
$$

If $f\in\mathcal H_U$, then testing against $C_0^\infty(U)$ and integrating by parts gives $\Delta f=0$ in $U$ in the [distributional derivative](../../../../../../distributional-derivative.md) sense. The [Weyl lemma](../../../../../../weyl-lemma.md) therefore gives a representative harmonic on $U$.

The [orthogonal decomposition by a closed subspace](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md) gives

$$
H_0^1(D)=H_0^1(U)\mathbin\oplus\mathcal H_U.
$$

Project the isonormal process defining $h$ onto these two orthogonal subspaces. The projections are jointly Gaussian and uncorrelated, hence [independent](../../../../../../independent-random-variables.md). The first projection is a zero-boundary Gaussian free field $h_U$ on $U$; the second is a random distribution $h^{\mathrm{har}}$ that is harmonic on $U$. Thus

$$
h=h_U+h^{\mathrm{har}},
$$

with independent summands. This proves the [Domain Markov property of the Gaussian free field](../../../../../../domain-markov-property-of-the-gaussian-free-field.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
