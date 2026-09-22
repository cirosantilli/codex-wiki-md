<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A strictly increasing differentiable concave [utility function](../../../../../../utility-function-split.md) on all of $\mathbb R$ has $U'(x)>0$ everywhere. Otherwise monotonicity and the decreasing derivative would make it constant on a right half-line. Its tangent at zero also shows $U(x)\to-\infty$ as $x\to-\infty$.

If $X$ has only one sign, the stated second alternative already holds. Otherwise both $\mathbb P(X<0)$ and $\mathbb P(X>0)$ are positive. As $\theta\to\infty$, $-U(\theta X)$ tends to infinity on $\{X<0\}$; as $\theta\to-\infty$, it does so on $\{X>0\}$. Since $-U\geq0$, [Fatou lemma](../../../../../../fatou-s-lemma.md) implies $F(\theta)\to-\infty$ at both ends. Continuity gives a finite maximizer $\theta_*$, and differentiability gives $F'(\theta_*)=0$.

For [optimal marginal utility as a one-period pricing density](../../../../../../optimal-marginal-utility-as-a-one-period-pricing-density.md), put $Z=U'(\theta_*X)$. It is strictly positive. On $\{|X|\geq1\}$ it is bounded by $|X|U'(\theta_*X)$, whose [expectation](../../../../../../expected-value.md) is finite by part ii. On $\{|X|<1\}$ continuity bounds $U'$ on the compact interval $[-|\theta_*|,|\theta_*|]$. Thus $Z$ is integrable and $XZ$ is absolutely integrable. **Consequently $\boxed{\mathbb E[XZ]=0}$**. Normalizing $Z$ by its positive [expectation](../../../../../../expected-value.md), if desired, makes it a probability density with the same zero pricing [expectation](../../../../../../expected-value.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
