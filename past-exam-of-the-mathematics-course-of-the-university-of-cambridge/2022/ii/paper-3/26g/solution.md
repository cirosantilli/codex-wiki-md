<h1 id="26g/solution">Solution</h1>

↑ **Parent:** [26G](../26g.md)

Convergence in distribution makes $(X_n)$ tight. Hence for every $\eta>0$ there is $M$ such that $\mathbb P(|X_n|>M)<\eta$ for all sufficiently large $n$. Since $Y_n-c\xrightarrow{P}0$,

$$
\mathbb P(|X_n(Y_n-c)|>\varepsilon)
\leq
\mathbb P(|X_n|>M)
+\mathbb P(|Y_n-c|>\varepsilon/M)
\longrightarrow\leq\eta.
$$

Letting $\eta\downarrow0$ gives $X_n(Y_n-c)\xrightarrow{P}0$. Also, the continuous-mapping theorem gives $cX_n\xrightarrow{d}cX$. Since

$$
X_nY_n=cX_n+X_n(Y_n-c),
$$

the [Slutsky theorem](../../../../../slutsky-theorem.md) yields

$$
\boxed{X_nY_n\xrightarrow{d}cX}.
$$

Now write the requested statistic as

$$
\frac{n^{-1/2}\sum_{i=1}^nZ_i}
{n^{-1}\sum_{i=1}^nZ_i^2}.
$$

The [central limit theorem](../../../../../central-limit-theorem.md) gives

$$
n^{-1/2}\sum_{i=1}^nZ_i\xrightarrow{d}N(0,1).
$$

Since $\mathbb E[Z_i^2]=1<\infty$, the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives

$$
\frac1n\sum_{i=1}^nZ_i^2\longrightarrow1
$$

almost surely, and therefore its reciprocal converges in probability to one. Applying the product result proves

$$
\boxed{
\frac{\sqrt n\sum_{i=1}^nZ_i}{\sum_{i=1}^nZ_i^2}
\xrightarrow{d}N(0,1)
}.
$$

This is a [self-normalized central limit theorem with a second-moment denominator](../../../../../self-normalized-central-limit-theorem-with-a-second-moment-denominator.md).

## ↑ Ancestors (10)

1. [26G](../26g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
