<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $f_j=\mathbb P(T=t_j)$ and $h_j=\mathbb P(T=t_j\mid T>t_{j-1})$. Since $S(t_{j-1})=\mathbb P(T>t_{j-1})$, the [discrete hazard](../../../../../../discrete-hazard.md) satisfies $h_j=f_j/S(t_{j-1})$. Hence

$$
S(t_j)=S(t_{j-1})-f_j=S(t_{j-1})(1-h_j).
$$

Starting from $S(0)=1$ and iterating, the [survival function](../../../../../../survival-function.md) is

$$
\boxed{S(t)=\prod_{j:t_j\le t}(1-h_j).}
$$

Under [independent censoring](../../../../../../independent-censoring.md), the [risk set](../../../../../../risk-set.md) just before $t_j$ gives the binomial conditional failure likelihood $h_j^{d_j}(1-h_j)^{n_j-d_j}$, whose maximizer is $\widehat h_j=d_j/n_j$. This gives the Kaplan–Meier estimator

$$
\boxed{\widehat S(t)=\prod_{j:t_j\le t}\left(1-\frac{d_j}{n_j}\right).}
$$

Failures at exactly $t$ are included because the target is $\mathbb P(T>t)$. Censored subjects contribute to earlier [risk sets](../../../../../../risk-set.md) and leave before later ones; they do not create a failure factor. The usual convention includes a subject censored at a tied failure time in the [risk set](../../../../../../risk-set.md) for that failure. Estimation beyond the last observed failure is limited by the available follow-up.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
