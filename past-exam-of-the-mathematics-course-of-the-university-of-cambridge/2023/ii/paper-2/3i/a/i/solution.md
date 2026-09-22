<h1 id="3i/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Bernoulli source](../../../../../../../bernoulli-source.md) is a sequence $(X_n)_{n\geq1}$ of [independent and identically distributed random variables](../../../../../../../independent-and-identically-distributed-random-variables.md) with a common [probability mass function](../../../../../../../probability-mass-function.md) on the finite [alphabet](../../../../../../../alphabet.md) $\mathcal A$.

The source is [reliably encodable at rate](../../../../../../../reliable-source-encoding-at-a-rate.md) $r$ if, for each block length $n$, there are an encoder with at most $2^{nr}$ outputs and a decoder such that the block error probability

$$
P\bigl(\widehat X_1^n\ne X_1^n\bigr)
$$

tends to zero as $n\to\infty$.

Its [information rate](../../../../../../../information-rate.md) is the limiting [information entropy](../../../../../../../information-entropy.md) per source symbol,

$$
h=\lim_{n\to\infty}\frac1nH(X_1,\ldots,X_n),
$$

when this [limit](../../../../../../../limit-of-a-function.md) exists.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3I](../../../3i.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
