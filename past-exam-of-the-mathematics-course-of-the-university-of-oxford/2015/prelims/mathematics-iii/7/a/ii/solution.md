<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assuming $g$ is [measurable](../../../../../../../measurability.md), applying it separately to [independent and identically distributed random variables](../../../../../../../independent-and-identically-distributed-random-variables.md) preserves those properties. Thus $W_i=g(X_i)$ have common [mean](../../../../../../../expected-value-split.md) $\mu_g$ and [variance](../../../../../../../variance-split.md) $\sigma_g^2$. For $\sigma_g^2>0$, the [central limit theorem](../../../../../../../central-limit-theorem.md) gives

$$
\frac{\sqrt n}{\sigma_g}\left(\frac1n\sum_{i=1}^ng(X_i)-\mu_g\right)\xrightarrow{d}N(0,1).
$$

Hence, for large $n$, the approximate [probability distribution](../../../../../../../probability-distribution-split.md) is

$$
\boxed{\frac1n\sum_{i=1}^ng(X_i)\ \approx\ N\left(\mu_g,\frac{\sigma_g^2}{n}\right).}
$$

The second argument is the [variance](../../../../../../../variance-split.md). If $\sigma_g^2=0$, this [sample mean](../../../../../../../sample-mean.md) equals $\mu_g$ [almost surely](../../../../../../../almost-sure-convergence.md), so the appropriate description is a [point mass](../../../../../../../point-mass.md) at $\mu_g$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
