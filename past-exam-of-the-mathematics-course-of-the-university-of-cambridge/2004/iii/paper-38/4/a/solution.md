<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $n$ be the number allocated to each arm and test equality of the two reconviction [probabilities](../../../../../../probability.md), with a specified target difference as the alternative. For equal independent binomial arms, put $\bar p=(p_A+p_B)/2$, $\Delta=p_A-p_B>0$, $v_0=2\bar p(1-\bar p)$ and $v_1=p_A(1-p_A)+p_B(1-p_B)$. Under the null the rejection boundary for $\widehat p_A-\widehat p_B$ is approximately $z_*\sqrt{v_0/n}$; under the planning alternative its mean is $\Delta$ and [variance](../../../../../../variance-split.md) is $v_1/n$. [statistical power](../../../../../../statistical-power.md) 0.8 is obtained approximately by requiring

$$
\Delta\sqrt n\ge z_*\sqrt{v_0}+z_{0.8}\sqrt{v_1}.
$$

Thus the [sample size for comparing two proportions](../../../../../../sample-size-for-comparing-two-proportions.md) is

$$
\boxed{n=\left\lceil\frac{[z_*\sqrt{v_0}+z_{0.8}\sqrt{v_1}]^2}{\Delta^2}\right\rceil,\qquad N=2n,}
$$

where $z_q=\Phi^{-1}(q)$, $z_*=z_{1-\alpha/2}$ for a [two-sided test](../../../../../../two-sided-hypothesis-test.md), or $z_{1-\alpha}$ for a prespecified one-sided superiority test. With $p_A=2/3$ and $p_B=1/3$, this simplifies to

$$
\boxed{n=\left\lceil\left(\frac{3z_*}{\sqrt2}+2z_{0.8}\right)^2\right\rceil.}
$$

For illustration only, at $\alpha=0.05$ this gives 35 per arm, 70 total, for a [two-sided test](../../../../../../two-sided-hypothesis-test.md), or 27 per arm, 54 total, for a [one-sided test](../../../../../../one-sided-hypothesis-test.md). No unique numerical count is specified until alpha and sidedness are fixed. These are normal planning approximations; an exact requirement can be checked by summing the probabilities, from the two independent [binomial distributions](../../../../../../binomial-distribution.md), of all tables in an exact test's rejection region and increasing $n$ until [statistical power](../../../../../../statistical-power.md) is at least 0.8.

This calculation detects a treatment difference when the effect equals the proposed target. It does not promise 80% [statistical power](../../../../../../statistical-power.md) to establish that the reduction is at least that target via a confidence bound when the true effect lies exactly at the target boundary. Such a different testing objective needs a separately specified null and planning alternative. Complete follow-up and ascertainment by [intention-to-treat analysis](../../../../../../intention-to-treat-analysis.md) are also required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
