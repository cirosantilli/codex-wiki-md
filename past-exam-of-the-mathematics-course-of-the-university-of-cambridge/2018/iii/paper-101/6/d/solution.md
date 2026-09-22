<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

We use three theorems for an [integral extension](../../../../../../integral-extension.md) $S\subseteq R$, none requiring [Noetherian](../../../../../../noetherian-ring.md) hypotheses. The [Lying-over theorem](../../../../../../lying-over-theorem.md) says that each [prime ideal](../../../../../../prime-ideal.md) $\mathfrak p$ of $S$ is $\mathfrak q\cap S$ for some [prime ideal](../../../../../../prime-ideal.md) $\mathfrak q$ of $R$. The [going-up theorem](../../../../../../going-up-theorem.md) says that if $\mathfrak p\subseteq\mathfrak p'$ in $S$ and $\mathfrak q\cap S=\mathfrak p$, there is $\mathfrak q'\supseteq\mathfrak q$ with $\mathfrak q'\cap S=\mathfrak p'$. The [incomparability theorem for integral extensions](../../../../../../incomparability-theorem-for-integral-extensions.md) says that comparable [prime ideals](../../../../../../prime-ideal.md) of $R$ with the same contraction to $S$ are equal.

Take any strict chain

$$
\mathfrak q_0\subsetneq\cdots\subsetneq\mathfrak q_n
$$

in $R$. The [contraction of an ideal](../../../../../../contraction-of-an-ideal.md) operation gives $\mathfrak p_j=\mathfrak q_j\cap S$, which are [prime ideals](../../../../../../prime-ideal.md) of $S$, by the proof in Question 1(b), and remain strictly increasing by the [incomparability theorem for integral extensions](../../../../../../incomparability-theorem-for-integral-extensions.md). Thus every chain length in $R$ occurs in $S$, giving $\dim R\leq\dim S$.

Conversely, take any strict chain $\mathfrak p_0\subsetneq\cdots\subsetneq\mathfrak p_n$ in $S$. Use the [Lying-over theorem](../../../../../../lying-over-theorem.md) to choose $\mathfrak q_0$ over $\mathfrak p_0$, then repeatedly use the [going-up theorem](../../../../../../going-up-theorem.md) to obtain $\mathfrak q_0\subseteq\cdots\subseteq\mathfrak q_n$ with the prescribed contractions. Each inclusion must be strict, since its contractions are distinct. Hence every chain length in $S$ occurs in $R$, giving $\dim S\leq\dim R$.

Taking suprema proves [integral extensions preserve Krull dimension](../../../../../../integral-extensions-preserve-krull-dimension.md):

$$
\boxed{\dim R=\dim S.}
$$

The argument works equally well when the dimensions are infinite, since it compares all finite chain lengths.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
