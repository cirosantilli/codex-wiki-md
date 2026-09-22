<h1 id="2/i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use base-two [logarithms](../../../../../../../logarithm.md). The [weakly typical sequence](../../../../../../../weakly-typical-sequence.md) definition is

$$
\boxed{\left|-\frac1n\log_2p(x^n)-H(X)\right|\leq\varepsilon},\qquad
p(x^n)=\prod_{j=1}^np(x_j).
$$

Equivalently, $2^{-n(H(X)+\varepsilon)}\leq p(x^n)\leq2^{-n(H(X)-\varepsilon)}$. By the [weak law of large numbers](../../../../../../../weak-law-of-large-numbers.md) applied to the [independent and identically distributed random variables](../../../../../../../independent-and-identically-distributed-random-variables.md) $-\log_2p(X_j)$, the probability of this [typical set](../../../../../../../typical-set.md) tends to one.

This captures the usual probability scale of a long sample, but it need not make every symbol frequency representative. For a fair binary source, every word has probability $2^{-n}$ and $H(X)=1$, so even the all-zero word is weakly typical. The [strongly typical sequence](../../../../../../../strongly-typical-sequence.md) definition additionally controls empirical symbol frequencies and excludes this word for small tolerance. Thus weak typicality agrees with the high-probability-set intuition, while allowing individually unrepresentative members.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [I](../../i.md)
3. [2](../../../2.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
