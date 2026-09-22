<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a concurrent comparison: test the same specimens for both [cocaine](../../../../../../cocaine.md) and [mephedrone](../../../../../../mephedrone.md), rather than treating the historical cocaine percentage as an exactly known 2010 parameter. Assume representative sampling of privates, effectively independent specimens, stable underlying rates during the sampling period, and sufficiently accurate assays. I use a two-sided 5% test of equal positive-test [probabilities](../../../../../../probability.md), with 80% [statistical power](../../../../../../statistical-power.md) at $p_C=0.010$ and $p_M=0.005$. This is a design to distinguish the rates at a twofold alternative; a significance test does not prove that their ratio is exactly two.

The paired design needs the joint positive-test distribution. For specimen $i$, write $C_i,M_i\in\{0,1\}$ and $D_i=C_i-M_i$. Put $q_{11}=P(C_i=M_i=1)$ and

$$
\delta=p_C-p_M=0.005,\qquad q=P(D_i\ne0)=p_C+p_M-2q_{11}.
$$

Then $\mathbb ED_i=\delta$ and $\operatorname{Var}(D_i)=q-\delta^2$. Under equal marginal rates, the two discordant outcomes have equal probabilities; conditional on the total number of discordant specimens, their split is a fair [binomial distribution](../../../../../../binomial-distribution.md). This gives the [McNemar test](../../../../../../mcnemar-s-test.md). Its large-sample version rejects for a sufficiently large absolute difference between the discordant counts, divided by their estimated standard deviation.

For planning, suppose simultaneous positives are negligible, so $q\simeq0.015$. Under the alternative the difference in positive counts has mean $n\delta$ and standard deviation $\sqrt{n(q-\delta^2)}$; the approximate upper null rejection boundary is $z_{0.975}\sqrt{nq}$. Requiring 80% upper-tail rejection probability gives the [paired binary sample size calculation](../../../../../../paired-binary-sample-size-calculation.md)

$$
\boxed{n\simeq\frac{\left[1.96\sqrt{0.015}+0.8416\sqrt{0.015-0.005^2}\right]^2}{0.005^2}\simeq4707.}
$$

**Add the mephedrone assay to about 5,000 existing tests, roughly ten weeks at 500 per week.** An exact conditional-power calculation under the negligible-overlap model gives about $77.6\%$ at 4,707 specimens and $80.2\%$ at 5,000, so the rounding also compensates for the conservative discrete test. If positivity for the two drugs were independent within a specimen, $q_{11}=0.00005$, giving a very similar requirement of about 4,676. For the stated marginal rates, $q\leq0.015$, so negligible overlap is a conservative variance choice within this approximation. Substantial co-use reduces the discordant proportion and changes the necessary size. Repeated tests on the same person, unit-level [clustered data](../../../../../../clustered-data.md) or inaccurate assays can instead reduce effective information and require more specimens.

A pre-specified one-sided 5% comparison would use $1.645$ in place of $1.96$ and require about 3,708 specimens before allowing for discreteness under the negligible-overlap assumption. These are different testing conventions. Treating the historical 1% as fixed would give a one-sample calculation, but would ignore uncertainty or changes in the actual 2010 cocaine rate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
