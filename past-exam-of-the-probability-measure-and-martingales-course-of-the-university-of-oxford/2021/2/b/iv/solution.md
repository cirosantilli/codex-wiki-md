<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $B_n=\{X_n>a_n\}$, the definition of the common [cumulative distribution function](../../../../../cumulative-distribution-function.md) gives

$$
\mathbb P(B_n)=1-F(a_n).
$$

The strict exceedance matters here: an [atom of a measure](../../../../../atom-measure-theory.md) at $a_n$ belongs to $\{X_n\leq a_n\}$, so it is already included in $F(a_n)$. The [events](../../../../../event.md) $B_n$ are mutually [independent events](../../../../../independent-events.md), since each depends on a separate member of the [independent random variables](../../../../../independent-random-variables.md) $X_n$.

If $\sum_n(1-F(a_n))<\infty$, [countable subadditivity](../../../../../countable-subadditivity-of-a-measure.md) gives, for every $N$,

$$
\mathbb P\left(\bigcup_{n\geq N}B_n\right)
\leq\sum_{n\geq N}(1-F(a_n))\longrightarrow0.
$$

[Continuity of probability](../../../../../continuity-of-probability.md) then gives $\mathbb P(\limsup_nB_n)=0$. This is the [First Borel-Cantelli lemma](../../../../../borel-cantelli-first-lemma.md) and does not need [independence](../../../../../independent-random-variables.md).

If the [series](../../../../../series-mathematics.md) diverges, [independence](../../../../../independent-random-variables.md) and $1-u\leq e^{-u}$ give, for every fixed $N$,

$$
\mathbb P\left(\bigcap_{n=N}^{M}B_n^c\right)
=\prod_{n=N}^{M}F(a_n)
\leq\exp\left(-\sum_{n=N}^{M}(1-F(a_n))\right)\longrightarrow0.
$$

Taking $M\to\infty$ shows that the [probability](../../../../../probability.md) of no exceedance after $N$ is zero. A [countable union](../../../../../countable-union.md) over $N$ shows that finitely many exceedances has [probability](../../../../../probability.md) zero. This is the [Second Borel-Cantelli lemma](../../../../../borel-cantelli-second-lemma.md). Together with the preceding [event](../../../../../event.md) equality, it proves

$$
\boxed{\mathbb P(A)=
\begin{cases}
0,&\sum_{n\geq1}(1-F(a_n))<\infty,\\
1,&\sum_{n\geq1}(1-F(a_n))=\infty.
\end{cases}}
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
