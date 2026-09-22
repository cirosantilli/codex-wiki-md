<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With $\mu_{\leq U}(d)=\mu(d)1_{d\leq U}$ and analogous notation for $\Lambda_{\leq V}$, [Vaughan identity](../../../../../../vaughan-s-identity.md) is

$$
\Lambda
=\Lambda_{\leq V}
+\mu_{\leq U}*\log
-\mu_{\leq U}*\Lambda_{\leq V}*1
+\mu_{>U}*\Lambda_{>V}*1.
$$

Thus, when $UV\leq N$,

$$
\begin{aligned}
\sum_{n\leq N}\Lambda(n)e(\alpha n^2)
={}&\sum_{n\leq V}\Lambda(n)e(\alpha n^2)\\
&+\sum_{d\leq U}\mu(d)\sum_{m\leq N/d}(\log m)e(\alpha d^2m^2)\\
&-\sum_{d\leq U}\mu(d)\sum_{m\leq V}\Lambda(m)
  \sum_{r\leq N/(dm)}e(\alpha d^2m^2r^2)\\
&+\sum_{\substack{d>U,\ m>V,\ r\geq1\\dmr\leq N}}
  \mu(d)\Lambda(m)e(\alpha d^2m^2r^2).
\end{aligned}
$$

The first term is short, the next two are Type I sums, and the last becomes a Type II [bilinear sum](../../../../../../bilinear-sum.md) after grouping variables and applying a [dyadic decomposition](../../../../../../dyadic-decomposition.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
