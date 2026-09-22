<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For fixed $\theta>0$, use the [Lyapunov condition](../../../../../../lyapunov-condition.md) for the independent centered epoch counts $Z_i=Y_{i+1}-\theta/i$. Their total [variance](../../../../../../variance-split.md) is $s_n^2=\theta H_{n-1}+\theta^2H_{n-1}^{(2)}\sim\theta\log n$.

Write $\mu_i=\theta/i$. Differentiating the [geometric distribution](../../../../../../geometric-distribution.md) [probability generating function](../../../../../../probability-generating-function.md) gives $\mathbb E[Y_{i+1}^3]=\mu_i+6\mu_i^2+6\mu_i^3$. Since $|Y_{i+1}-\mu_i|^3\le4Y_{i+1}^3+4\mu_i^3$, the sum of the centered absolute third [moments](../../../../../../moment.md) is $O(\log n)$. Consequently

$$
\frac{\sum_{i=1}^{n-1}\mathbb E|Z_i|^3}{s_n^3}=O((\log n)^{-1/2})\longrightarrow0.
$$

The [Lindeberg-Feller central limit theorem](../../../../../../lindeberg-feller-central-limit-theorem.md) applies through the [Lyapunov condition](../../../../../../lyapunov-condition.md), giving $(S-\theta H_{n-1})/s_n\xrightarrow{d}N(0,1)$. Now $\sqrt{\log n}\,s_n/H_{n-1}\to\sqrt\theta$, so the [Slutsky theorem](../../../../../../slutsky-theorem.md) proves the [asymptotic normality of the Watterson estimator](../../../../../../asymptotic-normality-of-the-watterson-estimator.md):

$$
\boxed{\sqrt{\log n}(\widehat\theta-\theta)\xrightarrow{d}N(0,\theta).}
$$

The limiting [variance](../../../../../../variance-split.md) is **$\theta$**. When $\theta=0$, every count vanishes and the limiting law is the point mass at zero.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
