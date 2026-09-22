<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $N(t)$ count observed failures and let $Y(t)$ be the [at-risk process](../../../../../../at-risk-process.md), counting subjects under observation and still alive immediately before $t$. Under [independent censoring](../../../../../../independent-censoring.md), a short interval of length $dt$ has conditional expected failure count $Y(t)h(t)\,dt=Y(t)\,dH(t)$. The estimating equation obtained by replacing the count expectation by its observation is $d\widehat H(t)=dN(t)/Y(t)$. Each distinct failure gives $\Delta N(a_m)=1$ and $Y(a_m)=r_m$, so the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) is

$$
\boxed{\widehat H_{\rm NA}(t)=\sum_{a_m\le t}\frac1{r_m}.}
$$

The same increment maximizes the local working [likelihood](../../../../../../likelihood-function.md) for a [Poisson distribution](../../../../../../poisson-distribution.md) with mean $r_m\Delta H_m$: differentiating $\Delta N_m\log(\Delta H_m)-r_m\Delta H_m$ gives $\Delta H_m=\Delta N_m/r_m$. The counting-process derivation explains why the [risk set](../../../../../../risk-set.md), rather than the initial sample size, supplies the denominator.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
