<h1 id="27j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [loss function](../../../../../../loss-function.md) $L(\theta,a)$ quantifies the cost of taking action $a$ when the parameter is $\theta$. A [decision rule](../../../../../../decision-rule.md) $d$ is a measurable map from the observation space to the action space (or, for randomized rules, a conditional action distribution). Its [risk function](../../../../../../risk-function.md) is $R(\theta,d)=\mathbb E_\theta L(\theta,d(X))$. For a prior [probability](../../../../../../probability.md) distribution $\pi$, its [Bayes risk](../../../../../../bayes-risk.md) is

$$
r(\pi,d)=\int_\Theta R(\theta,d)\,\pi(d\theta).
$$

A [minimax](../../../../../../minimax-decision-rule.md) rule minimizes $\sup_\theta R(\theta,d)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27J](../../27j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
