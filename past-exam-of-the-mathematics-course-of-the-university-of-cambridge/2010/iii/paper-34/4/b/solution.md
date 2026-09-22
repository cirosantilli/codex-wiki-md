<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the [null hypothesis](../../../../../../null-hypothesis.md) of equal [survival distributions](../../../../../../survival-distribution.md), the two groups have the same event hazard. Conditional on the current [risk set](../../../../../../risk-set.md) and one event, the event is in A with probability $r_j^A/(r_j^A+r_j^B)$ and in B with probability $r_j^B/(r_j^A+r_j^B)$. Consequently, whenever both groups are represented,

$$
\mathbb E_0\left[\frac{d_j^A}{r_j^A}-\frac{d_j^B}{r_j^B}\,\middle|\,\mathcal F_{a_j-},\text{one event}\right]
=\frac1{r_j^A+r_j^B}-\frac1{r_j^A+r_j^B}=0.
$$

Thus a weighted sum of differences in estimated hazard increments is centered under the null. Its sign reflects which group has more events relative to its numbers at risk. The weights may depend on event time and the preceding [risk sets](../../../../../../risk-set.md), but must not be chosen after seeing which group failed; otherwise this conditional-centering argument fails. Positive weights emphasize selected time regions without reversing an increment's direction. Such tests can have weak power against crossing hazards whose positive and negative contributions cancel.

Let $I_j=d_j^A$, so $d_j^B=1-I_j$. Its conditional null [variance](../../../../../../variance-split.md) is $r_j^Ar_j^B/(r_j^A+r_j^B)^2$. Since the unweighted hazard difference is $I_j(1/r_j^A+1/r_j^B)-1/r_j^B$, the conditional variance of its weighted contribution is $\omega_j^2/(r_j^Ar_j^B)$. Successive centered contributions form martingale differences. Their variance contributions add, providing a variance standardization for the test.

With the specified [log-rank weight](../../../../../../log-rank-weight.md), put $r_j=r_j^A+r_j^B$. Then

$$
\frac{r_j^Ar_j^B}{r_j}\left(\frac{d_j^A}{r_j^A}-\frac{d_j^B}{r_j^B}\right)
=\frac{r_j^Bd_j^A-r_j^Ad_j^B}{r_j}
=d_j^A-\frac{r_j^A}{r_j}.
$$

Therefore the displayed sum is exactly the unstandardized [log-rank statistic](../../../../../../log-rank-statistic.md)

$$
\boxed{U=\sum_j\left(d_j^A-\frac{r_j^A}{r_j}\right),\qquad
V=\sum_j\frac{r_j^Ar_j^B}{r_j^2}.}
$$

Its two-sided large-sample [log-rank test](../../../../../../log-rank-test.md) uses $U^2/V\Rightarrow\chi_1^2$ when $V>0$ and information is sufficient. If one group has no remaining subjects at some event time, its event contributes zero information. Use the final observed-minus-expected expression to define the contribution as zero; the original divided expression has an undefined $0/0$ and the log-rank weight becomes zero there. Thus strict positivity of the proposed weights implicitly restricts the comparison to event times when both groups are at risk. [Independent censoring](../../../../../../independent-censoring.md) and a valid conditional common-hazard model are required throughout.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
