<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $Y=\sqrt\tau$ and $V=X_\tau^*$. Splitting according to whether $V>\delta\lambda$, the [good-lambda bound for Brownian stopping time and maximum](../../../../../good-lambda-bound-for-brownian-stopping-time-and-maximum.md) gives

$$
\mathbb P(Y>\beta\lambda)\leq
\mathbb P(V>\delta\lambda)+\eta\mathbb P(Y>\lambda),
\qquad \eta=\frac{\delta^2}{\beta^2-1}.
$$

Integrate against the positive measure $d\Phi(\lambda)$. The [tail integral formula for expectation](../../../../../tail-integral-formula-for-expectation.md) in Stieltjes form yields

$$
\mathbb E\Phi(Y/\beta)
\leq\mathbb E\Phi(V/\delta)+\eta\mathbb E\Phi(Y).
$$

By [moderate growth](../../../../../moderate-growth.md), choose $K_\beta$ with $\Phi(\beta x)\leq K_\beta\Phi(x)$. Then

$$
\mathbb E\Phi(Y)
\leq K_\beta\mathbb E\Phi(V/\delta)
+K_\beta\eta\mathbb E\Phi(Y).
$$

Fix $\beta>1$ and choose $\delta$ small enough that $K_\beta\eta<1/2$. Absorb the last term and apply moderate growth once more to the fixed dilation $1/\delta$. This proves

$$
\boxed{\mathbb E\Phi(\sqrt\tau)\leq C_\Phi\mathbb E\Phi(X_\tau^*).}
$$

To avoid subtracting infinities, perform the argument first for $\tau\wedge n$, where Brownian maxima have all finite polynomial moments and moderate growth is at most polynomial, and then use [monotone convergence](../../../../../monotone-convergence-theorem.md). Applying the [Dambis-Dubins-Schwarz theorem](../../../../../dambis-dubins-schwarz-theorem.md) transfers this Brownian estimate to continuous local martingales, giving the lower-maximum side of the [Burkholder-Davis-Gundy inequalities](../../../../../burkholder-davis-gundy-inequalities.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
