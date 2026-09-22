<h1 id="27j/solution">Solution</h1>

↑ **Parent:** [27J](../27j.md)

In the normal form of a [Bayesian decision problem](../../../../../bayesian-decision-problem.md), choose a measurable [decision rule](../../../../../decision-rule.md) $\delta$ before seeing the data to minimize the prior [Bayes risk](../../../../../bayes-risk.md) $\mathbb EL(\Theta,\delta(X))$. In the extensive form, after observing $X=x$, choose an action minimizing posterior expected loss. [Conditional expectation](../../../../../conditional-expectation.md) makes these equivalent, subject to the usual measurable selection conditions. If $\Pi_x$ is the [posterior distribution](../../../../../bayesian-posterior.md) and $R_0(\Pi)=\inf_a\int L(\theta,a)\Pi(d\theta)$ is the best no-data loss, then

$$
\boxed{R_1=\mathbb E_X R_0(\Pi_X)\le R_0(\Pi).}
$$

The inequality follows by ignoring the data.

For a measurable region $S$, posterior or prior expected loss is $\int_S(c-\pi(\theta))\,d\theta$. It is minimized by including exactly the locations where the integrand is negative; including equality points is harmless. Thus the [highest density region](../../../../../highest-density-region.md) $S^*=\{\pi\ge c\}$ is a [Bayes act](../../../../../bayes-act.md) and

$$
\boxed{R_0(\Pi)=-\int(\pi-c)_+\,d\theta\le0.}
$$

For $N(\mu,\sigma^2)$, if $c\ge1/(\sigma\sqrt{2\pi})$ the answer is zero. Otherwise put $z_c=\sqrt{2\log[1/(c\sigma\sqrt{2\pi})]}$. The optimal interval is $[\mu-\sigma z_c,\mu+\sigma z_c]$, and

$$
\boxed{R_0=2c\sigma z_c-\bigl(2\Phi(z_c)-1\bigr).}
$$

For the specified prior and $c=1/2$, the prior density is everywhere below $c$, so $R_0=0$. Completing the square gives $\Theta\mid X=x\sim N(9x/10,1/10)$. Its peak is $\sqrt{10/(2\pi)}>1/2$, so a positive-measure region has posterior density strictly above $c$ and its optimal expected loss is strictly negative. That loss is independent of its mean, hence independent of $x$. Therefore **$R_1<0=R_0$**. Explicitly, with $z_c=\sqrt{2\log(2\sqrt{10/(2\pi)})}$, $R_1=z_c/\sqrt{10}-2\Phi(z_c)+1$.

## ↑ Ancestors (10)

1. [27J](../27j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
