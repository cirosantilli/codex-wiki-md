<h1 id="27i/solution">Solution</h1>

↑ **Parent:** [27I](../27i.md)

Write $R(\theta,\delta)=\mathbb E_\theta L(\theta,\delta(X))$ and $r(\pi,\delta)=\int R(\theta,\delta)\,d\pi(\theta)$. An [equaliser rule](../../../../../equalizer-rule.md) has constant risk $R(\theta,\delta)=c$. An [Extended Bayes rule](../../../../../extended-bayes-rule.md) has, for every $\varepsilon>0$, a proper prior $\pi$ such that $r(\pi,\delta)\le r^*(\pi)+\varepsilon$, where $r^*(\pi)=\inf_d r(\pi,d)$. If a rule has both properties, every competitor $d$ satisfies

$$
\sup_\theta R(\theta,d)\ge r(\pi,d)\ge r^*(\pi)\ge c-\varepsilon.
$$

Letting $\varepsilon\to0$ proves that its maximum risk $c$ is the [minimax risk](../../../../../minimax-risk.md).

For the given [normal distribution](../../../../../normal-distribution.md) model, completing the square in prior times likelihood gives the posterior $N(m,H^{-1})$, with $H=h_0+nh$ and $m=(h_0m_0+h\sum_i x_i)/H$. Another completion of the square gives

$$
\mathbb E\!\left[e^{-k(a-\theta)^2/2}\mid X=x\right]=\sqrt{\frac H{H+k}}\exp\!\left[-\frac{kH}{2(H+k)}(a-m)^2\right].
$$

This is maximized uniquely at $a=m$. Consequently the [Bayes act](../../../../../bayes-act.md) and posterior [posterior expected loss](../../../../../posterior-expected-loss.md) are

$$
\boxed{a_B=m,\qquad \rho_B(x)=1-\sqrt{\frac{h_0+nh}{h_0+nh+k}}.}
$$

The posterior loss is independent of $x$, so averaging over the predictive distribution gives the same value for the [Bayes risk](../../../../../bayes-risk.md) of this [Bayes decision rule](../../../../../bayes-decision-rule.md).

The [sample mean](../../../../../sample-mean.md) obeys $\bar X-\theta\sim N(0,(nh)^{-1})$, so its risk is the constant $c=1-\sqrt{nh/(nh+k)}$. Take any fixed $m_0$ and let the proper prior precisions $h_0\downarrow0$. The optimal [Bayes risks](../../../../../bayes-risk.md) just calculated tend to $c$, while the integrated risk of $\bar X$ is exactly $c$ for every prior. Thus its excess [Bayes risk](../../../../../bayes-risk.md) tends to zero: it is extended Bayes as well as equaliser. The preceding argument proves

$$
\boxed{\bar X\text{ is minimax, with risk }1-\sqrt{\frac{nh}{nh+k}}.}
$$

## ↑ Ancestors (10)

1. [27I](../27i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
