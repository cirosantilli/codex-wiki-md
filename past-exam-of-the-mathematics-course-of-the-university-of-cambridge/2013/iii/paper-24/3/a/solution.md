<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [independent increments](../../../../../../independent-increments.md) of [Brownian motion](../../../../../../brownian-motion-split.md), rather than merely checking that an [Itô formula](../../../../../../ito-s-lemma.md) drift vanishes. For $0\leq s<t$, put $h=t-s$ and write $B_t=B_s+Z$, where $Z$ is independent of $\mathcal F_s$ and has [normal distribution](../../../../../../normal-distribution.md) $N(0,h)$. Its first four [moments](../../../../../../moment.md) are $0,h,0,3h^2$. Therefore

$$
\begin{aligned}
\mathbb E(B_t^2\mid\mathcal F_s)&=B_s^2+h,\\
\mathbb E(B_t^3\mid\mathcal F_s)&=B_s^3+3hB_s,\\
\mathbb E(B_t^4\mid\mathcal F_s)&=B_s^4+6hB_s^2+3h^2.
\end{aligned}
$$

For the cubic expression, the coefficient of $B_s$ after conditioning is $3(t-s)+\alpha(t)$, so $\alpha(t)=-3t$ makes it $\alpha(s)$. For the quartic expression, choose $\beta(t)=-6t$. Its conditioned coefficient of $B_s^2$ is then $6(t-s)-6t=-6s$. The constant term becomes

$$
3(t-s)^2-6t(t-s)+\gamma(t),
$$

which equals $3s^2$ when $\gamma(t)=3t^2$. Thus a standard choice is

$$
\boxed{\alpha(t)=-3t,\qquad\beta(t)=-6t,\qquad\gamma(t)=3t^2.}
$$

The resulting [stochastic processes](../../../../../../stochastic-process-split.md) are [Hermite polynomial martingales](../../../../../../space-time-hermite-polynomial.md) $H_3(B_t,t)$ and $H_4(B_t,t)$. They are genuine integrable [martingales](../../../../../../martingale-split.md), since Gaussian [moments](../../../../../../moment.md) are finite at every finite time and the displayed conditional identities establish the [martingale](../../../../../../martingale-split.md) property directly.

The choice is not unique. Constants $c,d,e\in\mathbb R$ give the valid family $\alpha(t)=c-3t$, $\beta(t)=d-6t$, and $\gamma(t)=3t^2-dt+e$: these add $cB_t$ to the cubic [martingale](../../../../../../martingale-split.md) and $d(B_t^2-t)+e$ to the quartic one. The boxed choice sets these harmless additions to zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
