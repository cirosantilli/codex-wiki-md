<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Z=1$ mean membership in the structural-zero component. Under the fitted [zero-inflated Poisson regression](../../../../../../../zero-inflated-poisson-regression.md), $P(Y=0\mid Z=1)=1$, whereas $P(Y=0\mid Z=0)=e^{-\mu}$. By [Bayes' theorem](../../../../../../../bayes-theorem.md), the [posterior structural-zero probability](../../../../../../../posterior-structural-zero-probability.md) is

$$
P(Z=1\mid Y=0)=\frac{\pi}{\pi+(1-\pi)e^{-\mu}}.
$$

Using the printed predictions for this patient gives

$$
\boxed{\frac{0.4448758}{0.4448758+(1-0.4448758)\,0.8007976}\approx0.50019.}
$$

**The fitted conditional probability is about $50.0\%$.** It is larger than the prior fitted structural-zero probability $0.4448758$, because observing no episodes increases the probability of latent membership in that component. The interpretation “never at risk” is the model's structural class; an observed six-month zero alone does not identify the class with certainty.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
