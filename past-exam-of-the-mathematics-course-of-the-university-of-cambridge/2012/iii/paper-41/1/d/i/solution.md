<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\mu_i=\alpha+\beta z_i+\gamma^{\mathsf T}x_i$ and let $f_i(y)=\sigma^{-1}\phi((y-\mu_i)/\sigma)$ be the [normal distribution](../../../../../../../normal-distribution.md) density. Set $q_j(y)=\operatorname{expit}(\eta_j+\theta y)$, where $q_j$ is the probability that attempt $j$ is unsuccessful conditional on the preceding attempts being unsuccessful. This is a [sequential response selection model](../../../../../../../sequential-response-selection-model.md). For first-attempt success, the observed outcome and attempt count contribute

$$
\boxed{L_i=f_i(y_i)[1-q_1(y_i)]
=\frac{\phi((y_i-\mu_i)/\sigma)}{\sigma[1+e^{\eta_1+\theta y_i}]}.}
$$

This [likelihood](../../../../../../../likelihood-function.md) conditions on baseline and assignment; the displayed response probabilities do not use $d_i$. No factor for random allocation is needed when conditioning on its realized value.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Paper 41](../../../../paper-41-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
