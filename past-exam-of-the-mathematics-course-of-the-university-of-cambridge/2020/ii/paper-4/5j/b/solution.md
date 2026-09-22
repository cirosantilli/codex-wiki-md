<h1 id="5j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The intercept-only model has $49$ residual degrees of freedom, so the sample size is $50$. The one-covariate model and full model therefore have respectively $48$ and $47$ residual degrees of freedom. The completed sequential [analysis of variance](../../../../../../analysis-of-variance.md) table has

$$
\begin{array}{c|c|c|c|c|c}
&\mathrm{Res.Df}&\mathrm{RSS}&\mathrm{Df}&\mathrm{Sum\ of\ Sq}&F\\ \hline
1&49&164.448&&&\\
2&48&30.831&1&164.448-30.831&\dfrac{164.448-30.831}{30.817/47}\\
3&47&30.817&1&30.831-30.817&\dfrac{30.831-30.817}{30.817/47}
\end{array}
$$

Thus the missing sums of squares are $133.617$ and $0.014$, and the corresponding [F-statistics](../../../../../../f-statistic.md) are approximately $203.8$ and $0.0214$. The first p-value is below $2\times10^{-16}$; the second is approximately $0.8845$. The tiny second increment is consistent with the reported [t-test](../../../../../../student-s-t-test.md) because, for one added coefficient, the partial F-statistic equals the squared t-statistic up to displayed rounding.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5J](../../5j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
