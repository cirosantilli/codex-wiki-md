<h1 id="m/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\overline X_n=n^{-1}\sum_iX_i$ and write $\sigma^2=\operatorname{Var}(X_1)<\infty$. Independence gives $\mathbb E\overline X_n=\mu$ and $\operatorname{Var}(\overline X_n)=\sigma^2/n$. Apply part (b) to the nonnegative variable $(\overline X_n-\mu)^2$, which is the [Chebyshev inequality](../../../../../chebyshev-s-inequality.md):

$$
\mathbb P(|\overline X_n-\mu|>\varepsilon)
\leq\frac{\sigma^2}{n\varepsilon^2}\longrightarrow0.
$$

Thus **$\overline X_n\to\mu$ in [probability](../../../../../probability.md)**, proving the finite-[variance](../../../../../variance-split.md) [weak law of large numbers](../../../../../weak-law-of-large-numbers.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [M](../../../m.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
