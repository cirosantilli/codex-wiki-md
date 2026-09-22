<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Integrating the positive component's [normal distribution](../../../../../../normal-distribution.md) prior gives its [prior predictive distribution](../../../../../../bayesian-model-evidence.md):

$$
\boxed{Y_i\mid+,V\sim N(0,1+V).}
$$

The negative component gives $Y_i\mid-\sim N(0,1)$. Let $f_1(y)=\phi_{1+V}(y)$ and $f_0(y)=\phi_1(y)$ denote those centred normal densities. The [point-null mixture prior](../../../../../../point-null-mixture-prior.md) assigns component odds $q/(1-q)$, so the [posterior odds](../../../../../../posterior-odds.md) of the positive component are

$$
\boxed{O_i(y_i)=\frac q{1-q}\frac1{\sqrt{1+V}}
\exp\left\{\frac{Vy_i^2}{2(1+V)}\right\}.}
$$

Its [posterior probability](../../../../../../posterior-probability.md) is $O_i/(1+O_i)$. Evidence depends on $y_i^2$, so large effects of either sign favour the positive component. This is the marginal distribution before observing $y_i$, not the posterior predictive law for a second observation conditional on it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
