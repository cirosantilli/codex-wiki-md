<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Work internally in the ground model and write $P=\operatorname{Levy}(\aleph_0,\lambda)$. Conditions are finite partial [functions](../../../../../../function-split.md) with the coordinate-wise value bounds in the PDF, ordered by inclusion, so compatible conditions agree on their common domain and their union is a common strengthening.

Suppose there were $\lambda$ many pairwise incompatible conditions. Each fixed finite domain carries fewer than $\lambda$ possible [functions](../../../../../../function-split.md): it uses finitely many [ordinals](../../../../../../ordinal.md) below $\lambda$, and each coordinate has fewer than $\lambda$ choices. Regularity therefore lets us select $\lambda$ distinct domains. The finite-set form of the [generalized delta-system lemma](../../../../../../generalized-delta-system-lemma.md) gives a subfamily of size $\lambda$ with common intersection $r$. There are fewer than $\lambda$ possible value assignments to the finite root $r$. Regularity gives a further subfamily of size $\lambda$ agreeing on the root. Any two of its conditions have a union in $P$, contradicting incompatibility. Thus **$P$ has the $\lambda$-chain condition**. Strong inaccessibility is more than is needed for this finite-support argument; regular uncountability suffices.

For each $0<\alpha<\lambda$ and $n<\omega$, requiring $(n,\alpha)$ to be in the domain is dense. For each $\xi<\alpha$, requiring $\xi$ to occur as a value at some $(n,\alpha)$ is also dense: choose a fresh $n$ and extend the condition. Hence the generic union defines, for each such $\alpha$, a [surjection](../../../../../../surjective-function.md) $g_\alpha:\omega\to\alpha$. Every ground [ordinal](../../../../../../ordinal.md) below $\lambda$ is therefore countable in $M[G]$.

By the chain condition and the cardinal-preservation argument, $\lambda$ remains an uncountable [cardinal](../../../../../../cardinal-number.md) in the extension; the same small-value argument preserves its regularity as well. All [ordinals](../../../../../../ordinal.md) are unchanged. Since every smaller [ordinal](../../../../../../ordinal.md) is countable and $\lambda$ is not,

$$
\boxed{\aleph_1^{M[G]}=\lambda.}
$$

This is the [finite Lévy collapse to omega-one](../../../../../../finite-levy-collapse-to-omega-one.md). The dense-set construction proves the collapse below $\lambda$, while the chain condition is what prevents collapsing $\lambda$ itself.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
