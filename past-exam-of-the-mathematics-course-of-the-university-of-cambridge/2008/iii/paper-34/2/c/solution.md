<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $a>0$ and $n\geq2$, let $A_n(a)=\{X_n^2>a\log n\}$. Symmetry of the [standard normal distribution](../../../../../../standard-normal-distribution.md) and the [Mills ratio](../../../../../../mills-ratio.md) asymptotic just proved give

$$
\mathbb P(A_n(a))=2\bigl[1-\Phi(\sqrt{a\log n})\bigr]
\sim\sqrt{\frac{2}{\pi a}}\frac{n^{-a/2}}{\sqrt{\log n}}.
$$

For $a>2$ the [series](../../../../../../series-mathematics.md) of these [probabilities](../../../../../../probability.md) converges, since its terms are eventually bounded by a constant times the convergent [p-series](../../../../../../p-series.md) $n^{-a/2}$. For $0<a<2$ it diverges: choose $r$ strictly between $a/2$ and one, and use $(\log n)^{-1/2}\geq n^{-(r-a/2)}$ for sufficiently large $n$, reducing to the divergent [p-series](../../../../../../p-series.md) $n^{-r}$. At $a=2$ it still diverges, as the [integral test](../../../../../../integral-test-for-convergence.md) gives

$$
\int_2^R\frac{dt}{t\sqrt{\log t}}
=2\bigl(\sqrt{\log R}-\sqrt{\log2}\bigr)\longrightarrow\infty.
$$

For $a>2$, the first [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) makes $A_n(a)$ occur only finitely often. For $0<a\leq2$, independence of the [random variables](../../../../../../random-variable-split.md) makes the [events](../../../../../../event.md) $A_n(a)$ independent, so the second [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) makes them occur infinitely often [almost surely](../../../../../../almost-sure-convergence.md). Apply these conclusions simultaneously at $a=2+1/k$ for positive integers $k$, and at $a=2$. On the resulting [probability](../../../../../../probability.md)-one [event](../../../../../../event.md), the [limit superior](../../../../../../limit-superior.md) is at most every $2+1/k$ and at least two. Therefore the [Gaussian sample limsup at logarithmic scale](../../../../../../gaussian-sample-limsup-at-logarithmic-scale.md) is

$$
\boxed{\limsup_{n\to\infty}\frac{X_n^2}{\log n}=2\quad\text{almost surely}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
