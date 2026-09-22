<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [events](../../../../../../event.md) $A_n$, define their [limit superior](../../../../../../limit-superior.md) by

$$
A_\infty=\limsup_n A_n=\bigcap_{N\geq1}\bigcup_{n\geq N}A_n.
$$

It is the [event](../../../../../../event.md) that infinitely many $A_n$ occur. The two [Borel-Cantelli lemmas](../../../../../../borel-cantelli-lemmas.md) are as follows: if $\sum_n\mathbb P(A_n)<\infty$, then $\mathbb P(A_\infty)=0$, without any independence assumption; if the $A_n$ are independent and $\sum_n\mathbb P(A_n)=\infty$, then $\mathbb P(A_\infty)=1$.

For the first assertion, the [union bound](../../../../../../boole-s-inequality.md) gives, for every $N$,

$$
\mathbb P(A_\infty)\leq\mathbb P\!\left(\bigcup_{n\geq N}A_n\right)
\leq\sum_{n\geq N}\mathbb P(A_n).
$$

The tail of a convergent nonnegative [series](../../../../../../series-mathematics.md) tends to zero, proving the first [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md).

For the second assertion, independence and $1-u\leq e^{-u}$ for $0\leq u\leq1$ give

$$
\mathbb P\!\left(\bigcap_{n=N}^K A_n^c\right)
=\prod_{n=N}^K(1-\mathbb P(A_n))
\leq\exp\!\left(-\sum_{n=N}^K\mathbb P(A_n)\right)\longrightarrow0.
$$

By [continuity of probability](../../../../../../continuity-of-probability.md), $\mathbb P(\bigcap_{n\geq N}A_n^c)=0$. The [event](../../../../../../event.md) that only finitely many $A_n$ occur is the countable [union](../../../../../../set-union.md) of these zero-probability [events](../../../../../../event.md) over $N$. Its [probability](../../../../../../probability.md) is zero. This proves the second [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md), and hence both requested assertions:

$$
\boxed{\sum_n\mathbb P(A_n)<\infty\Rightarrow\mathbb P(A_\infty)=0,\qquad
\text{independence and }\sum_n\mathbb P(A_n)=\infty\Rightarrow\mathbb P(A_\infty)=1.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
