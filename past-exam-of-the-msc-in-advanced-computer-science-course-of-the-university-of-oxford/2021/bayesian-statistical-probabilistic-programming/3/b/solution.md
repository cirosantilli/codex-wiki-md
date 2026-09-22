<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An idealized underlying [probability space](../../../../../probability-space-split.md) is

$$
\Omega=(0,60)\times(1,20)\times\mathbb R^{25},\qquad
\mathbb P=\operatorname{Unif}(0,60)\otimes\operatorname{Unif}(1,20)\otimes N(0,1)^{\otimes25},
$$

with the product [Borel sigma-algebra](../../../../../borel-sigma-algebra.md). Its 27 independent random coordinates are $\mu$, $\sigma$, twenty past standard-normal noises, and five future standard-normal noises. Define $T_i(\omega)=\mu+\sigma\varepsilon_i$. Sampling an unknown [variance](../../../../../variance-split.md) does not mean drawing a new [variance](../../../../../variance-split.md) on each day; a single draw of $\sigma^2$ applies to all durations in a trace.

Let $A$ be the [event](../../../../../event.md) that the first twenty durations satisfy their corresponding observed inequalities. The observations are the twenty late/early labels, conditional on the fixed departure thresholds. They are not exact values of the latent $T_i$. The posterior [probability measure](../../../../../probability-measure.md) on traces is

$$
\mathbb P_A(B)=\mathbb P(B\mid A)=\frac{\mathbb P(B\cap A)}{\mathbb P(A)}.
$$

Here $\mathbb P(A)>0$: at every interior parameter pair each strict normal-tail [probability](../../../../../probability.md) lies in $(0,1)$, so their finite product has positive prior integral.

The returned outcome is

$$
Y(\omega)=\mathbf1\{T_{21}>30,\ldots,T_{25}>30\}\in\{0,1\}.
$$

Thus **the underlying [sample space](../../../../../sample-space.md) has dimension 27, the successful output space is $\{0,1\}$, and the observations define the conditioning event $A$**. The desired output [probability distribution](../../../../../probability-distribution-split.md) is the [pushforward measure](../../../../../pushforward-measure.md) of $\mathbb P_A$ under $Y$. Rejection is an implementation device, not a third scientific answer: `None` is discarded before forming the conditional output law.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
