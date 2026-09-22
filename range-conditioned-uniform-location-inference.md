# Range-conditioned uniform location inference

↑ **Parent:** [Ancillary statistic](ancillary-statistic.md)

For independent observations uniform on $(\theta-1/2,\theta+1/2)$, let $U$ and $V$ be the sample minimum and maximum, $R=V-U$, and $C=(U+V)/2$. For $n\ge2$ their joint [density](density.md) in $(c,r)$ is $n(n-1)r^{n-2}$ on $0<r<1$, $|c-\theta|<(1-r)/2$. Integrating over $c$ gives $f_R(r)=n(n-1)r^{n-2}(1-r)$, independent of $\theta$, so $R$ is an [ancillary statistic](ancillary-statistic.md). Moreover $C\mid R=r$ is uniform on $(\theta-(1-r)/2,\theta+(1-r)/2)$. Consequently

$$
\left[C-\frac{(1-\alpha)(1-R)}2,\ C+\frac{(1-\alpha)(1-R)}2\right]
$$

is an exact conditional $(1-\alpha)$ [confidence interval](confidence-interval.md) for $\theta$. The realized range determines the appropriate precision, although the range is not itself evidence about the value of $\theta$.

## ↑ Ancestors (6)

1. [Ancillary statistic](ancillary-statistic.md)
2. [Sufficient statistic](sufficient-statistic.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38/6/iii/solution.md)
