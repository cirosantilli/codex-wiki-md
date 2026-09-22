<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [Wilcoxon signed-rank test](../../../../../../wilcoxon-signed-rank-test.md), assume independent observations from a continuous distribution symmetric about the specified $\theta_0$. Form $D_i=X_i-\theta_0$, rank the absolute differences $|D_i|$, and add the ranks of positive differences:

$$
W_+=\sum_i R_i\mathbf1_{\{D_i>0\}},\qquad W_-=\frac{n(n+1)}2-W_+.
$$

Under the continuous null there are no zeros or tied absolute values with positive probability. Symmetry makes the signs independent fair signs conditional on the magnitudes, so the exact null distribution is that of $\sum_{j=1}^n jB_j$ for independent $B_j\sim\operatorname{Bernoulli}(1/2)$. In particular

$$
\boxed{\mathbb E_0W_+=\frac{n(n+1)}4,\qquad\operatorname{Var}_0(W_+)=\frac{n(n+1)(2n+1)}{24},\qquad\mathbb E_0z^{W_+}=2^{-n}\prod_{j=1}^n(1+z^j).}
$$

The coefficients of this polynomial give exact tail probabilities, or they can be computed by recursively adding a rank with probability one half. A two-sided test rejects for unusually small $\min(W_+,W_-)$, equivalently for extreme $W_+$ on either side of its center. Choose symmetric tail cutoffs with total null probability at most $\alpha$; discrete boundary randomization can attain size exactly $\alpha$. An exact conservative two-sided p-value is $\min\{1,2\min(\mathbb P_0(W_+\leq w),\mathbb P_0(W_+\geq w))\}$. For a positive-location alternative use the upper tail, and for a negative-location alternative use the lower tail.

For large samples, centering and scaling by the displayed mean and standard deviation gives an asymptotic standard normal statistic. This follows from the independent weighted Bernoulli representation, because the largest squared weight is negligible relative to the sum of squared weights. A continuity correction improves the normal tail approximation. With observed zero differences, omit them in the usual convention; tied absolute differences receive average ranks, and the conditional null variance is then one quarter of the sum of squared assigned ranks, not automatically the no-tie formula.

Symmetry is essential: having median $\theta_0$ alone need not make the signs independent of the magnitudes, and so does not justify these exact critical values. The test is particularly useful for location shifts in symmetric families. It is a valid test of the stated symmetry null, but is not an omnibus procedure guaranteed to detect every asymmetric alternative.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
