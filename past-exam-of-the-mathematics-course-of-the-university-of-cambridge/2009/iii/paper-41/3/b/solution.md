<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [Cox proportional-hazards model](../../../../../../cox-proportional-hazards-model.md) as $h_i(t)=h_0(t)u_i$, where $u_i=\exp(\beta^Tz_i)$ is the [hazard multiplier](../../../../../../hazard-multiplier.md) and $h_0$ is the unspecified [baseline hazard](../../../../../../baseline-hazard.md). At an untied event time $t_j$, let $R_j$ be the [risk set](../../../../../../risk-set.md) immediately before the event and $i_j$ its failing individual. With [independent censoring](../../../../../../independent-censoring.md) conditional on the [covariates](../../../../../../covariate.md), the [conditional probability](../../../../../../conditional-probability.md) that individual $i$ supplies the next event, given an event at that time and the [risk set](../../../../../../risk-set.md), is obtained by dividing its instantaneous event rate by the aggregate rate:

$$
\Pr(i_j=i\mid\text{one event at }t_j,R_j)
=\frac{h_0(t_j)u_i}{\sum_{k\in R_j}h_0(t_j)u_k}
=\frac{u_i}{\sum_{k\in R_j}u_k}.
$$

More precisely this is the limit of the [conditional probability](../../../../../../conditional-probability.md) for one event in a short interval; simultaneous events have smaller-order probability in the continuous model. Multiplication of these successive conditional contributions gives the [Cox partial likelihood](../../../../../../cox-partial-likelihood.md)

$$
\boxed{L_P(\beta)=\prod_{j:\,\text{event}}\frac{\exp(\beta^Tz_{i_j})}{\sum_{k\in R_j}\exp(\beta^Tz_k)}.}
$$

Censored individuals remain in each [risk set](../../../../../../risk-set.md) until their [censoring](../../../../../../censoring-statistics.md) time but supply no numerator. Conditioning removes the [baseline hazard](../../../../../../baseline-hazard.md); this is a [partial likelihood](../../../../../../partial-likelihood.md) for $\beta$, rather than a complete [likelihood](../../../../../../likelihood-function.md) for event and [censoring](../../../../../../censoring-statistics.md) times.

**Ties require an observation model or an approximation.** Suppose a recorded tie hides the order of $d$ continuous events, with no intervening entry or [censoring](../../../../../../censoring-statistics.md). Put $D$ for the tied event set and $S=\sum_{i\in R}u_i$. An exact marginal contribution for the coarsened ranks is the sum of the ordinary rank contributions over every possible order:

$$
L_{\mathrm{rank},D}=\sum_{\pi\in\operatorname{Perm}(D)}
\prod_{q=0}^{d-1}\frac{u_{\pi_{q+1}}}{S-\sum_{r=1}^{q}u_{\pi_r}}.
$$

For example, if $A,B$ fail together while $C$ remains at risk, the two possible orders give

$$
L_{\mathrm{rank},\{A,B\}}=
\frac{u_Au_B}{S}\left(\frac1{S-u_A}+\frac1{S-u_B}\right),
\qquad S=u_A+u_B+u_C.
$$

The [risk set](../../../../../../risk-set.md) is depleted after the first of the two events. This expression concerns the missing event order; it is not the full [likelihood](../../../../../../likelihood-function.md) of an interval in which the events occurred.

Convenient alternatives are the [Breslow approximation for tied event times](../../../../../../breslow-approximation-for-tied-event-times.md) and the [Efron approximation for tied event times](../../../../../../efron-approximation-for-tied-event-times.md):

$$
L_{B,D}=\frac{\prod_{i\in D}u_i}{S^d},\qquad
L_{E,D}=\frac{\prod_{i\in D}u_i}{\prod_{q=0}^{d-1}[S-(q/d)\sum_{i\in D}u_i]}.
$$

The first keeps the initial denominator at every event; the second removes an average share of the tied-event multipliers successively. In the example their denominators are $S^2$ and $S[S-(u_A+u_B)/2]$. These conventional partial-likelihood factors omit multiplicities independent of $\beta$, which do not affect its estimate; they should not be mistaken for normalized probabilities of the unordered event set.

For genuinely discrete event times there is another exact construction. If individual event odds are proportional to $u_i$, conditioning on exactly $d$ events gives the [exact tied-set conditional likelihood](../../../../../../exact-tied-set-conditional-likelihood.md)

$$
L_{\mathrm{set},D}=\frac{\prod_{i\in D}u_i}{\sum_{A\subseteq R:\,|A|=d}\prod_{i\in A}u_i}.
$$

For the same three individuals this is $u_Au_B/(u_Au_B+u_Au_C+u_Bu_C)$. It is not generally equal to the continuous-time rank sum: the assumptions differ.

Large tie groups make naive summation over $d!$ orders or $\binom{|R|}{d}$ subsets impractical. Recursion helps with the subset denominator, and Breslow or Efron avoids exhaustive enumeration. However, extensive ties can also indicate that time is measured too coarsely for an exact continuous-time ordering to be a useful target.

For example, if patients are assessed only at annual visits, use one row per patient-year still at risk and model the probability $p_{ij}$ of an event in that interval. A [grouped proportional-hazards model](../../../../../../grouped-proportional-hazards-model.md) follows directly by integrating the hazard over the interval, with [covariates](../../../../../../covariate.md) constant there:

$$
p_{ij}=1-\exp[-\Delta H_{0j}\exp(\beta^Tz_i)],
\qquad
\boxed{\log[-\log(1-p_{ij})]=\alpha_j+\beta^Tz_i,\quad
\alpha_j=\log\Delta H_{0j}.}
$$

Fit the resulting person-period [likelihood](../../../../../../likelihood-function.md), with [Bernoulli distributions](../../../../../../bernoulli-distribution.md) for the interval event indicators and interval-specific intercepts. Many events in the same year are then ordinary observations rather than a combinatorial ordering problem. This requires a compatible interval-observation scheme and appropriate [independent censoring](../../../../../../independent-censoring.md); it avoids pretending that unobserved within-year event times are known.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
