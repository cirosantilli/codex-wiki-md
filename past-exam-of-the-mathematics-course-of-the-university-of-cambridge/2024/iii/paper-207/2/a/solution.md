<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\widehat p_k=X_k/n_k$, where $X_k\sim\operatorname{Binomial}(n_k,p_k)$ independently, and put

$$
\widehat V=\frac{\widehat p_1(1-\widehat p_1)}{n_1}
+\frac{\widehat p_0(1-\widehat p_0)}{n_0}.
$$

The [Wald statistic](../../../../../../wald-test.md) is $Z=(\widehat p_1-\widehat p_0)/\sqrt{\widehat V}$. The [central limit theorem](../../../../../../central-limit-theorem.md) and [Slutsky theorem](../../../../../../slutsky-theorem.md) give $Z\dot\sim N(0,1)$ under $H_0$. When $p_1-p_0=\delta^*>0$,

$$
\boxed{Z\dot\sim N\!\left(
\frac{\delta^*}{\sqrt{p_1(1-p_1)/n_1+p_0(1-p_0)/n_0}},1
\right).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
