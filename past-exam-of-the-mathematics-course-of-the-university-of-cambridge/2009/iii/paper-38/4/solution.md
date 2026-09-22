<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the one-sided [Wilcoxon rank sum test](../../../../../mann-whitney-u-test.md), suppose $X_1,\ldots,X_m$ and $Y_1,\ldots,Y_n$ are independent samples, iid within each sample, with continuous distributions. The [null hypothesis](../../../../../null-hypothesis.md) is a common distribution. For a lower-tail alternative, the $X$ distribution is stochastically smaller. In the common-shape location model $X\overset d=Y+\delta$, this is $H_0:\delta=0$ against $H_1:\delta<0$; in that model it also compares [medians](../../../../../median.md). Without a location-family assumption, equality or inequality of medians alone is not the defining rank-sum hypothesis.

Rank all $N=m+n$ observations from smallest to largest and form $W_X=\sum_{i=1}^m\operatorname{rank}(X_i)$. Reject for small $W_X$. Under $H_0$, the labels are exchangeable, so every subset of $m$ of the $N$ ranks is equally probable. The [exact null distribution of a rank sum](../../../../../exact-null-distribution-of-a-rank-sum.md) is therefore

$$
\Pr_0(W_X=w)=\frac{\#\{S\subseteq\{1,\ldots,N\}:|S|=m,\ \sum_{k\in S}k=w\}}{\binom Nm}.
$$

Enumerate these subsets, or use the coefficient of $z^mt^w$ in $\prod_{k=1}^N(1+zt^k)$. An efficient recursion adds rank $k$ either to the selected sample or not: $a_{k,h,w}=a_{k-1,h,w}+a_{k-1,h-1,w-k}$, starting with $a_{0,0,0}=1$. The lower-tail [P-value](../../../../../p-value.md) is $\Pr_0(W_X\leq W_{\mathrm{obs}})$. A nonrandomized level-$\alpha$ test chooses a lower-tail rejection region whose null probability is at most $\alpha$.

The shifted [Mann–Whitney U test](../../../../../mann-whitney-u-test.md) statistic is $U_X=W_X-m(m+1)/2$. It counts pairs with $Y_j<X_i$, so the same lower-tail test uses small $U_X$. The distinction is important for these S-Plus outputs: **the printed values are raw rank sums**, not the shifted statistic used by some other software.

For the one-sided [Wilcoxon signed-rank test](../../../../../wilcoxon-signed-rank-test.md), the pairs $(U_i,V_i)$ are independent between individuals but their two measurements may be dependent. Let $D_i=U_i-V_i$, and assume the differences are iid, continuous and symmetric about a common location $\delta$. Test $H_0:\delta=0$ against $H_1:\delta<0$. Rank the absolute differences and use

$$
W_+=\sum_{i:D_i>0}\operatorname{rank}(|D_i|).
$$

Under the null, conditional on their absolute values, the signs are independent fair signs. Every subset of ranks therefore has probability $2^{-n}$ of being the positive-sign subset, giving the exact null distribution of $W_+$. Reject for small $W_+$ and calculate the lower-tail probability. Its null mean and variance are $n(n+1)/4$ and $n(n+1)(2n+1)/24$. The symmetry assumption is essential: zero median by itself does not give this law. With zeros or ties, omit zero differences in the usual signed-rank version and use average ranks for ties, adjusting the distribution accordingly. The paired test is not appropriate for the independent RHR samples here.

For the experienced participants, let $X$ denote RHR1 running time and $Y$ denote RHR2 running time. The [null hypothesis](../../../../../null-hypothesis.md) is identical running-time distributions; under the location interpretation it is zero RHR1-minus-RHR2 shift. The one-sided alternative is a negative shift, so RHR1 participants tend to run faster. With $m=n=13$, the printed statistic is

$$
\boxed{W_X=135,\qquad U_X=135-\frac{13\cdot14}{2}=44,\qquad p=0.0193.}
$$

At $5\%$, reject the null in favour of faster RHR1 running times. The sample [medians](../../../../../median.md) $11.52$ and $12.78$ minutes agree with that direction; their difference is descriptive, not the rank-sum test statistic.

For the new participants the same independent-sample [Wilcoxon rank sum test](../../../../../mann-whitney-u-test.md) compares eight RHR1 times against nine RHR2 times, again with a lower-tail alternative. Here

$$
\boxed{W_X=58,\qquad U_X=58-\frac{8\cdot9}{2}=22,\qquad p=0.0998.}
$$

The [exact null distribution of a rank sum](../../../../../exact-null-distribution-of-a-rank-sum.md) gives this probability. It does not reject at $5\%$, although it is just below $10\%$. The data suggest the same direction but are less decisive; this is not evidence that the two new-participant distributions are equal.

The final command pools the experienced and new RHR1 samples into $m=21$ observations, and the corresponding RHR2 samples into $n=22$. It repeats the lower-tail rank-sum comparison on these two pooled groups. `exact=F` requests a [normal approximation for a rank sum](../../../../../normal-approximation-for-a-rank-sum.md) with a continuity correction. Without ties,

$$
\mathbb E_0W_X=\frac{m(N+1)}2=462,\qquad
\operatorname{var}_0W_X=\frac{mn(N+1)}{12}=1694.
$$

The lower-tail statistic is $(W_X-462+1/2)/\sqrt{1694}$, with the usual tie-adjusted variance if ties occur. The supplied output is

$$
\boxed{Z=-2.2233,\qquad p=\Phi(-2.2233)=0.0131,}
$$

where $\Phi$ is the standard [normal distribution](../../../../../normal-distribution.md) function. Thus the pooled test rejects at $5\%$. The unreported pooled ranks must be formed afresh: the within-cohort raw rank sums cannot simply be added because pooling introduces cross-cohort comparisons.

Taken together, there is evidence that participants classified as RHR1 have shorter running times among the experienced men and in the pooled sample. The smaller new-participant samples give weaker evidence in the same direction. A significant result in one cohort and a nonsignificant result in another does not itself prove that their RHR effects differ. Pooling also assumes a meaningful pooled comparison; if programme duration changes the distributions, a cohort-adjusted analysis would be more informative. These observational comparisons do not establish that the fitness programme caused the differences, and none of the three tests directly compares experienced participants with new participants.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
