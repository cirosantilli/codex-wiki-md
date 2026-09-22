<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $h=H^2(P_0,P_1)$ with the paper's normalized [Hellinger distance](../../../../../hellinger-distance.md). The [Hellinger affinity](../../../../../hellinger-affinity.md) is

$$
A(P_0,P_1)=\int\sqrt{p_0p_1}\,d\mu=1-h,\qquad0\leq A(P_0,P_1)\leq1.
$$

The last bound follows from the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and the unit integrals of the two [probability density functions](../../../../../probability-density-function.md). Using a common dominating [probability measure](../../../../../probability-measure.md), for example $(P_0+P_1)/2$, makes the product calculation immediate. The [probability density functions](../../../../../probability-density-function.md) of the [product measures](../../../../../product-measure.md) factor, and [Tonelli's theorem](../../../../../tonelli-theorem.md) gives

$$
A(P_0^n,P_1^n)
=\int\prod_{i=1}^n\sqrt{p_0(x_i)p_1(x_i)}\,d\mu^{\otimes n}(\mathbf x)
=A(P_0,P_1)^n.
$$

The [Squared Hellinger distance](../../../../../squared-hellinger-distance.md) is independent of the choice of common dominating measure, so this calculation applies to the original distributions. We obtain the exact identity and then apply [Bernoulli's inequality](../../../../../bernoulli-s-inequality.md):

$$
\boxed{H^2(P_0^n,P_1^n)=1-(1-h)^n\leq nh=nH^2(P_0,P_1).}
$$

For completeness, the scalar bound follows by induction: $(1-h)^1=1-h$, and multiplying $(1-h)^n\geq1-nh$ by the nonnegative $1-h$ gives $(1-h)^{n+1}\geq1-(n+1)h+nh^2\geq1-(n+1)h$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
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
