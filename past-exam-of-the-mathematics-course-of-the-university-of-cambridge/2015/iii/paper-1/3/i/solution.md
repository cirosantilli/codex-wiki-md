<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [integral extension](../../../../../../integral-extension.md) $R\subseteq T$ means every $t\in T$ satisfies a [monic polynomial](../../../../../../monic-polynomial.md)

$$
t^d+a_{d-1}t^{d-1}+\cdots+a_0=0,\qquad a_j\in R.
$$

To prove the [Lying-over theorem](../../../../../../lying-over-theorem.md), localize at $S=R\setminus P$. The injection $R_P\hookrightarrow S^{-1}T$ remains injective, and $S^{-1}T$ is integral over $R_P$: a monic relation for $t$ divided by suitable powers of $s$ gives one for $t/s$. This is a nonzero ring, so choose a [maximal ideal](../../../../../../maximal-ideal.md) $M$ of it.

The contraction of $M$ to $R_P$ is maximal. To see this directly, a [field](../../../../../../field.md) integral over a subring forces that subring to be a [field](../../../../../../field.md). For nonzero $a$ in the subring, $a^{-1}$ is integral; multiply its monic equation of degree $d$ by $a^{d-1}$ to express $a^{-1}$ as a polynomial in $a$ with coefficients in the subring. Apply this to the [integral extension](../../../../../../integral-extension.md)

$$
R_P/(M\cap R_P)\ \subseteq\ (S^{-1}T)/M.
$$

Since $R_P$ is a [local ring](../../../../../../local-ring.md) with unique [maximal ideal](../../../../../../maximal-ideal.md) $PR_P$, we obtain $M\cap R_P=PR_P$.

Contract $M$ to $T$, obtaining a [prime ideal](../../../../../../prime-ideal.md) $Q$. Its contraction to $R$ is the contraction of $PR_P$, namely $P$. **Thus**

$$
\boxed{\text{there exists }Q\in\operatorname{Spec}T\text{ with }Q\cap R=P.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
