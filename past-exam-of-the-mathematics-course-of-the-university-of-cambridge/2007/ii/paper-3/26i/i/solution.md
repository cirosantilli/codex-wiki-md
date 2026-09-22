<h1 id="26i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a prior $\Pi$ and loss $L$, the [Bayes risk](../../../../../../bayes-risk.md) of a rule $d$ is $r(\Pi,d)=\int\mathbb E_\theta L(\theta,d(X))\,\Pi(d\theta)$. A [Bayes decision rule](../../../../../../bayes-decision-rule.md) minimizes this integrated risk. An [Extended Bayes rule](../../../../../../extended-bayes-rule.md) is a rule whose excess over the optimal [Bayes risk](../../../../../../bayes-risk.md) can be made arbitrarily small by a suitable proper prior: for every $\varepsilon>0$ some $\Pi$ has $r(\Pi,d)\leq\inf_{d'}r(\Pi,d')+\varepsilon$, with finite risks.

Condition on the observation and use iterated expectation. A rule is Bayes precisely when it chooses a minimizer of the posterior expected loss almost surely, up to the usual measurability requirement. Under squared Euclidean loss, with a finite posterior [second moment](../../../../../../second-moment.md), write $m=\mathbb E[\theta\mid X]$. The identity

$$
\mathbb E[\|\theta-a\|^2\mid X]
=\mathbb E[\|\theta-m\|^2\mid X]+\|m-a\|^2
$$

shows that **the Bayes rule is the [posterior mean](../../../../../../posterior-mean.md)**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [26I](../../26i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
