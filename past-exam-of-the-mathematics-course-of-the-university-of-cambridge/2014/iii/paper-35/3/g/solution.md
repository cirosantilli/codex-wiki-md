<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

With equal model [prior probabilities](../../../../../../prior-probability.md), [Bayes factor](../../../../../../bayes-factor.md) updating gives $w_0=B_{01}/(1+B_{01})$ and $w_1=1/(1+B_{01})$. The [Bayesian model averaging](../../../../../../bayesian-model-averaging.md) [posterior density](../../../../../../posterior-density.md) is therefore

$$
\boxed{p(\beta\mid y)=\frac{B_{01}}{1+B_{01}}p_0(\beta\mid y)+\frac1{1+B_{01}}p_1(\beta\mid y).}
$$

This is a two-component [mixture model](../../../../../../mixture-model.md) of the [normal distributions](../../../../../../normal-distribution.md) already derived. For the numerical observation above, **$w_0\simeq0.10829$ and $w_1\simeq0.89171$**. Consequently it is predominantly the wide-model posterior, not predominantly the narrow one.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
