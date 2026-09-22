<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Discarding zero observations and resolving ties is unnecessary with probability one under the stated independent continuous model. Rank the absolute observations from $1$ to $n$, let $R_i$ be the rank of $|X_i|$, and form the positive [Wilcoxon signed-rank statistic](../../../../../wilcoxon-signed-rank-statistic.md)

$$
W^+=\sum_iR_i\mathbf1_{X_i>0}.
$$

Reject the [null hypothesis](../../../../../null-hypothesis.md) for large $W^+$. Under symmetry about zero, each sign is a fair independent binary variable, independent of all the absolute values. To see this [independence](../../../../../independent-random-variables.md), for every [measurable](../../../../../measurability.md) positive set $B$, symmetry gives $\Pr(X\in B)=\Pr(X\in-B)=\tfrac12\Pr(|X|\in B)$. [Independence](../../../../../independent-random-variables.md) of observations then gives [independence](../../../../../independent-random-variables.md) of the whole sign vector from the absolute-value vector. Conditional on those absolute values, relabeling by rank therefore gives

$$
W^+\overset d=\sum_{r=1}^n rB_r,\qquad B_r\text{ independent Bernoulli}(1/2).
$$

The null distribution is consequently independent of the unknown symmetric shape. Its [probability generating function](../../../../../probability-generating-function.md) is $2^{-n}\prod_{r=1}^n(1+z^r)$, so the coefficient of $z^w$ gives the exact probability of $W^+=w$. Choose an upper critical value with null tail probability at most the desired level, or randomize at the boundary to obtain that level exactly. The observed upper-tail probability is an exact one-sided [p-value](../../../../../p-value.md). A positive translation raises each [Walsh average](../../../../../walsh-average.md), as established below, so this upper-tail rule has the correct direction against positive centers for every fixed symmetric shape.

The independent-sign representation proves

$$
\boxed{E_0W^+=\frac12\sum_{r=1}^n r=\frac{n(n+1)}4,\qquad \operatorname{Var}_0W^+=\frac14\sum_{r=1}^n r^2=\frac{n(n+1)(2n+1)}{24}.}
$$

The asymptotic null distribution, stated without proof, is

$$
\boxed{\frac{W^+-n(n+1)/4}{\sqrt{n(n+1)(2n+1)/24}}\ \xrightarrow{d}\ N(0,1).}
$$

This supplies the usual upper [normal distribution](../../../../../normal-distribution.md) critical value when exact calculation is inconvenient; for the discrete upper tail $\Pr(W^+\ge c)$, use $c-1/2$ in the [continuity correction](../../../../../continuity-correction.md).

For exact equivalence with the proposed [statistic](../../../../../statistic.md), reorder the observations so $|X_{(1)}|<\cdots<|X_{(n)}|$. Partition the unordered pairs, including diagonals, by the member with larger absolute value. The block belonging to $X_{(r)}$ consists of the $r-1$ pairs with an earlier member and its diagonal pair. For an earlier member $X_{(j)}$, the strict inequality $|X_{(j)}|<|X_{(r)}|$ means the sign of $X_{(j)}+X_{(r)}$ is the sign of $X_{(r)}$; the diagonal sum has that same sign. Thus the entire block supplies exactly $r$ positive averages when $X_{(r)}>0$, and none otherwise. Summing the blocks proves

$$
\boxed{\#\{(i,j):i\le j,\ (X_i+X_j)/2>0\}=\sum_{r=1}^n r\mathbf1_{X_{(r)}>0}=W^+.}
$$

The two tests therefore have exactly the same [statistic](../../../../../statistic.md), critical values and [p-values](../../../../../p-value.md), not merely the same limiting distribution. The [Walsh averages](../../../../../walsh-average.md) are dependent, so their positivity indicators must not instead be treated as an independent binomial sample. For a translation $X_i=Z_i+\theta$ of any null-symmetric sample, every [Walsh average](../../../../../walsh-average.md) increases by $\theta$; their positive count is nondecreasing, which also verifies the direction of the one-sided test.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
