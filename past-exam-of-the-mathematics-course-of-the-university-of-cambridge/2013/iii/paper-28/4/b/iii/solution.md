<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With a new count $x_{n+1}$, the updated [Bühlmann credibility estimate](../../../../../../../buhlmann-credibility-premium.md) is $(C_n+x_{n+1}+12)/(n+7)$. Subtracting the previous estimate gives the [sequential Bühlmann credibility update](../../../../../../../sequential-buhlmann-credibility-update.md)

$$
\widehat m_{n+1}-\widehat m_n=\frac{x_{n+1}-\widehat m_n}{n+7}.
$$

Therefore the new estimate is strictly smaller exactly when

$$
\boxed{x_{n+1}<\widehat m_n=\frac{C_n+12}{n+6}.}
$$

Because a claim count is a nonnegative integer, the equivalent set is $x_{n+1}\in\{0,1,\ldots,\lceil\widehat m_n\rceil-1\}$. A count equal to the previous estimate leaves it unchanged; a larger count increases it. The comparison is with the previous credibility estimate, which already combines the prior population mean and the observed mean.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
