<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The experimental unit for comparing the treatments is the pot: its two plants form a pair. Let $D_i=C_i-S_i$ be cross-fertilised minus self-fertilised height in pot $i$, for $i=1,\ldots,15$. The paired [Wilcoxon signed-rank test](../../../../../wilcoxon-signed-rank-test.md) assumes independent differences with a continuous distribution symmetric about a location $\delta$. Its null is $\delta=0$, with the one-sided formulation $\delta\le0$, against $\delta>0$. Under this location model it asks whether cross-fertilisation produces a positive shift within a pot. The location is a [median](../../../../../median.md), and also a mean if it exists; a hypothesis merely about a [median](../../../../../median.md) without symmetry does not justify the signed-rank null distribution.

Test 1 uses this paired test and its exact distribution. Form the fifteen differences, omit any zero differences, rank their absolute values, and sum the [statistical ranks](../../../../../rank-of-an-observation.md) belonging to positive differences. That positive-rank sum is the reported $V=96$. Tied absolute differences receive average [statistical ranks](../../../../../rank-of-an-observation.md). Under the symmetric zero-location null, conditional on their magnitudes, the signs are independent fair signs. The exact upper-tail probability is obtained from all sign allocations to the observed [statistical ranks](../../../../../rank-of-an-observation.md): with fifteen nonzero differences there are $2^{15}$ equiprobable allocations. For untied absolute differences the rank weights are $1,\ldots,15$; ties would require the corresponding conditional rank weights. The reported probability of a positive-rank sum at least as large as observed is $0.0206$. No [normal approximation](../../../../../normal-approximation.md) is used.

Test 2 makes exactly the same paired comparison and has the same null and alternative hypotheses. `exact=F` replaces the exact distribution by a [normal approximation](../../../../../normal-approximation.md) with a [continuity correction](../../../../../continuity-correction.md). Under an untied null the positive-rank sum has

$$
E(V)=\frac{n(n+1)}4,\qquad\operatorname{Var}(V)=\frac{n(n+1)(2n+1)}{24}.
$$

More generally, conditional on the nonzero absolute [statistical ranks](../../../../../rank-of-an-observation.md) $r_i$, its [variance](../../../../../variance-split.md) is $\tfrac14\sum_i r_i^2$. The upper-tail correction places the boundary half a lattice unit below the observed statistic. Standardizing gives the reported $Z=2.0163$, and its approximate $p$-value is $1-\Phi(Z)=0.0219$. Thus the slight difference from Test 1 reflects approximation, not a different scientific question.

Test 3 omits `paired=T`, so it is the unpaired [Wilcoxon rank sum test](../../../../../mann-whitney-u-test.md). Its usual distribution-free null is that two independent samples have the same continuous distribution. In a common-shape location model this is a zero location difference, against a positive cross-minus-self shift. More generally “greater” directs the test towards the cross distribution being shifted upwards; it does not turn the test into a general comparison of means or medians for arbitrary unequal shapes.

To form its statistic, pool the thirty heights, rank them together with averaged [statistical ranks](../../../../../rank-of-an-observation.md) for ties, and add the cross-group [statistical ranks](../../../../../rank-of-an-observation.md) to get $R_C$. Equivalently use $U=R_C-n_C(n_C+1)/2$. Under independent untied samples,

$$
E(U)=\frac{n_Cn_S}{2},\qquad\operatorname{Var}(U)=\frac{n_Cn_S(n_C+n_S+1)}{12}.
$$

If the pooled ties have sizes $t_h$ and $N=n_C+n_S$, the [variance](../../../../../variance-split.md) becomes

$$
\frac{n_Cn_S}{12}\left\{N+1-\frac{\sum_h(t_h^3-t_h)}{N(N-1)}\right\}.
$$

Subtract the null mean and the upper-tail [continuity correction](../../../../../continuity-correction.md), then divide by this null standard deviation. This procedure gives the reported rank-sum $Z=3.0105$. Its approximate one-sided probability is $1-\Phi(Z)=0.0013$. This describes how the statistic and probability are obtained without reconstructing the unprinted heights.

For the statistician, **use the paired analysis, preferably the exact Test 1 for these fifteen pairs**. The independent units are the pots, while the two heights within a pot share growing conditions and cannot be treated as independent samples. Test 2 is a reasonable approximation to the same paired test and agrees closely. Test 3 discards the matching and uses a null [variance](../../../../../variance-split.md) that assumes [independence](../../../../../independent-random-variables.md) between the samples, so its smaller $p$-value is not a reason to prefer it. The appropriate paired result gives evidence at $5\%$, but not at $1\%$, that cross-fertilised plants have a positive height shift relative to their paired self-fertilised plants, subject to the symmetry assumption for differences.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
