<h1 id="28j/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For each $i$, let $\widehat\theta_{(-i)}$ be the same estimator computed after deleting $X_i$, and put $\overline\theta_{(-)}=n^{-1}\sum_i\widehat\theta_{(-i)}$. The [jackknife bias correction](../../../../../../../jackknife-bias-correction.md) is

$$
\boxed{\widehat\theta_{\mathrm J}
=n\widehat\theta_n-(n-1)\overline\theta_{(-)}.}
$$

Its bias is

$$
nB_n(\theta_0)-(n-1)B_{n-1}(\theta_0)=O(n^{-2}),
$$

so the leading $a/n$ term has been removed and the bias is smaller than that of $\widehat\theta_n$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [28J](../../../28j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
