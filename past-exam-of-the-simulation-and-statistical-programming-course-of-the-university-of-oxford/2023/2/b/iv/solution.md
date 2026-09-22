<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The proposal's [normalization of a probability distribution](../../../../../normalization-of-a-probability-distribution.md) is

$$
\boxed{Z_q=\int_{\mathbb R}e^{-|x|}\,dx=2,\qquad q(x)=\tfrac12e^{-|x|}.}
$$

This is the [Laplace distribution](../../../../../laplace-distribution.md) with location zero and scale one. For example, generate its magnitude from the [exponential distribution](../../../../../exponential-distribution.md) with rate one and give it an [independent](../../../../../independent-random-variables.md) fair sign. The target is the [standard normal distribution](../../../../../standard-normal-distribution.md), with $Z_p=\sqrt{2\pi}$.

To obtain the tight envelope, let $t=|x|$. By [completing the square](../../../../../completing-the-square.md),

$$
\frac{\widetilde p(x)}{\widetilde q(x)}
=e^{-t^2/2+t}=e^{1/2}e^{-(t-1)^2/2}\leq e^{1/2}.
$$

Equality occurs at $x=\pm1$, so $\boxed{M_*=\sqrt e}$ is the smallest valid envelope constant. It maximizes the acceptance [probability](../../../../../probability.md) for this fixed proposal. The supplied lower bound must be clipped at zero to satisfy the algorithm's nonnegativity requirement:

$$
\boxed{h(x)=\max\{0,1-x^2/2\}.}
$$

This is valid because $e^{-s}\geq1-s$ for $s\geq0$, while $\widetilde p$ is everywhere positive. Its [support](../../../../../support.md) is $[-\sqrt2,\sqrt2]$.

Here is the fully specified [squeeze rejection sampling](../../../../../squeeze-rejection-sampling.md) procedure. Draw $Y$ with [probability density function](../../../../../probability-density-function.md) $q(y)=e^{-|y|}/2$, independently draw $U\sim\operatorname{Unif}(0,1)$, and compute $H=\max(0,1-Y^2/2)$ and $B=\sqrt e\,e^{-|Y|}$. If $U\leq H/B$, return $Y$ immediately. Otherwise evaluate $P=e^{-Y^2/2}$, independently draw $V\sim\operatorname{Unif}(0,1)$, and return $Y$ if $V\leq(P-H)/(B-H)$. On rejection restart with fresh draws. In this example $B>H$ everywhere, so the residual denominator is positive.

Avoiding a target evaluation means accepting at the first test. Its unconditional [probability](../../../../../probability.md) for one proposal is

$$
\begin{aligned}
\mathbb P(\text{no target evaluation})
&=\int_{\mathbb R}q(y)\frac{h(y)}{M\widetilde q(y)}\,dy\\
&=\frac1{2\sqrt e}\int_{-\sqrt2}^{\sqrt2}(1-y^2/2)\,dy\\
&=\boxed{\frac{2\sqrt2}{3\sqrt e}\approx0.571843.}
\end{aligned}
$$

For comparison, the overall acceptance [probability](../../../../../probability.md) is $\sqrt{2\pi}/(2\sqrt e)=\sqrt{\pi/(2e)}\approx0.760173$. The first-stage saving $0.571843$ is the fraction of proposals requiring no target evaluation, including both eventual accepted and rejected proposals in the denominator; it is not conditional on acceptance.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
