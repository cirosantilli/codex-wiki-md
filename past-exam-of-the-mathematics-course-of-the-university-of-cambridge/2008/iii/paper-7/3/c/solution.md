<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $A$ is a [regular local ring](../../../../../../regular-local-ring.md), $\dim A=d$ is finite. Choose a chain of [prime ideals](../../../../../../prime-ideal.md) of length $d$,

$$
\mathfrak p_0\subsetneq\mathfrak p_1\subsetneq\cdots\subsetneq\mathfrak p_d=\mathfrak m.
$$

Such a chain exists because the supremum defining this finite integer [Krull dimension](../../../../../../krull-dimension.md) is attained; a maximal-length chain in a [local ring](../../../../../../local-ring.md) ends at its [maximal ideal](../../../../../../maximal-ideal.md).

For each $i$, the [ideal](../../../../../../ideal.md) $\mathfrak p_i$ is finitely generated because $A$ is [Noetherian](../../../../../../noetherian-ring.md). This ensures that its extension $\mathfrak p_iB$ consists precisely of series all of whose coefficients lie in $\mathfrak p_i$: if $\mathfrak p_i=(b_1,\ldots,b_r)$, write each coefficient as $\sum_j b_jc_{jn}$ and gather them into the finitely many series $\sum_n c_{jn}x^n$. Thus coefficient reduction gives

$$
B/\mathfrak p_iB\cong(A/\mathfrak p_i)[[x]].
$$

The coefficient ring $A/\mathfrak p_i$ is an [integral domain](../../../../../../integral-domain.md), and so is its [formal power series ring](../../../../../../formal-power-series.md): the first nonzero coefficient of a product is the product of the first nonzero coefficients of its factors. Hence each $\mathfrak p_iB$ is prime. Also $\mathfrak p_iB\cap A=\mathfrak p_i$, so the strict inclusions persist upon extension. Finally, $x\notin\mathfrak mB$, since its image in $B/\mathfrak mB\cong k[[x]]$ is nonzero. We obtain the prime chain

$$
\mathfrak p_0B\subsetneq\cdots\subsetneq\mathfrak p_dB=\mathfrak mB\subsetneq\mathfrak mB+(x)=I
$$

of length $d+1$. Therefore $\dim B\geq d+1$. Together with part (b),

$$
\boxed{\dim A[[x]]=d+1.}
$$

Its [embedding dimension](../../../../../../embedding-dimension.md) is also $d+1$, by part (b), so $B$ is itself a [regular local ring](../../../../../../regular-local-ring.md). This proves that [formal power series preserve regular local rings](../../../../../../formal-power-series-preserve-regular-local-rings.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
