<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use two translated [uniform distributions](../../../../../continuous-uniform-distribution.md), with parameters $0$ and $a=1/(2n)$. Their distance in the usual [metric](../../../../../metric.md) is $a$, so take the separation radius $\delta=a/2=1/(4n)$ and the [loss function](../../../../../loss-function.md) $\Phi(r)=r^2$. The supplied testing reduction, equivalently the [Le Cam two-point lemma](../../../../../le-cam-two-point-lemma.md), and part (a)(i) imply

$$
m_n\geq\delta^2\frac{1-V(U_0^n,U_a^n)}2
=\frac{a^2}{8}\bigl[1-V(U_0^n,U_a^n)\bigr].
$$

To see the reduction directly, turn any [estimator](../../../../../estimator.md) into a binary [hypothesis test](../../../../../statistical-hypothesis-test-split.md) by choosing the closer of $0$ and $a$. If the test is wrong, the absolute estimation error is at least $a/2$. The worst [quadratic risk](../../../../../quadratic-risk.md) is at least its average over these two parameters, giving precisely this bound.

Under [Lebesgue measure](../../../../../lebesgue-measure.md) on $\mathbb R^n$, the two sample [probability density functions](../../../../../probability-density-function.md) are the indicators of the cubes $[0,1]^n$ and $[a,a+1]^n$. Their intersection is $[a,1]^n$, of volume $(1-a)^n$. Therefore

$$
1-V(U_0^n,U_a^n)
=\int\min(p_0^{(n)},p_a^{(n)})\,d\mathbf x
=(1-a)^n\geq1-na=\frac12,
$$

where the inequality is [Bernoulli's inequality](../../../../../bernoulli-s-inequality.md). Consequently

$$
\boxed{m_n\geq\frac{a^2}{16}=\frac1{64n^2},\qquad C=\frac1{64}.}
$$

This also fits the [Hellinger distance](../../../../../hellinger-distance.md) approach: the two one-sample affinities give $H^2(U_0,U_a)=a$, while equal-height indicator densities imply $V(U_0^n,U_a^n)=H^2(U_0^n,U_a^n)$. Part (a)(ii) thus yields the same bound $V\leq na=1/2$. The change of support produces [Squared Hellinger distance](../../../../../squared-hellinger-distance.md) proportional to $a$, explaining the parameter scale $a\asymp n^{-1}$ and [quadratic risk](../../../../../quadratic-risk.md) scale $n^{-2}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../../split.md)
6. [Algorithmic foundations of learning course of the University of Oxford](../../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
