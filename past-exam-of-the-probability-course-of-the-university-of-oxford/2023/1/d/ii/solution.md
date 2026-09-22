<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Taking [logarithms](../../../../../logarithm.md) of the product gives

$$
\boxed{W_n=\exp\left(-\sum_{j=1}^nV_j\right).}
$$

By part (d)(i), $V_j=E_j-\log b$ in [probability distribution](../../../../../probability-distribution-split.md), where $E_j$ has the [exponential distribution](../../../../../exponential-distribution.md) of rate one. Thus $\mathbb E|V_j|\leq1+|\log b|<\infty$ and $\mathbb EV_j=1-\log b$. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives

$$
\frac1n\log W_n=-\frac1n\sum_{j=1}^nV_j\longrightarrow\log b-1\quad\text{almost surely}.
$$

If $b<e$, choose $\delta=(1-\log b)/2>0$. Eventually $\log W_n\leq-\delta n$, so $W_n\leq e^{-\delta n}\to0$. If $b>e$, choose $\delta=(\log b-1)/2>0$; eventually $W_n\geq e^{\delta n}\to\infty$. Therefore

$$
\boxed{W_n\to0\text{ a.s. if }0<b<e;\qquad W_n\to\infty\text{ a.s. if }b>e.}
$$

In particular, the second range cannot have [almost sure convergence](../../../../../almost-sure-convergence.md) to zero. This is the [almost-sure growth rate of independent products](../../../../../almost-sure-growth-rate-of-independent-products.md). At $b=e$ the logarithmic limit is zero, which by itself decides neither behavior; that boundary case is not requested.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
