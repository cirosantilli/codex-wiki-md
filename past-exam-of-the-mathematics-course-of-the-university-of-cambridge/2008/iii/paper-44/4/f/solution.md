<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Keep a tree-specific log asymptote $a_i$ with a normal population distribution, but use one shared location $b$ and one shared positive growth coefficient $k$. For example, with fixed prior constants chosen on meaningful scales:

```
mean.a ~ dnorm(m.a, precision.a.prior)
sd.a ~ dnorm(0, precision.sd.a) T(0,)
precision.a <- 1 / pow(sd.a, 2)
b ~ dnorm(m.b, precision.b.prior)
k ~ dnorm(m.k, precision.k.prior) T(0,)
sigma ~ dnorm(0, precision.sigma.prior) T(0,)
precision.y <- 1 / pow(sigma, 2)
for (i in 1:5) {
    a[i] ~ dnorm(mean.a, precision.a)
    for (j in 1:7) {
        fitted[i,j] <- exp(a[i]) / (1 + exp(-b - k*t[j]))
        Y[i,j] ~ dnorm(fitted[i,j], precision.y)
    }
}
```

Here the transformed days `t[j]` are supplied as data. This is Model C: only the log asymptote is a [random effect](../../../../../../random-effect.md), while location and growth rate are shared. The prior constants are fixed inputs, and the truncations give positive standard deviations and an increasing growth curve. One can retain the original error-precision prior for a comparison matching the supplied fits; the code above illustrates a more interpretable positive-scale alternative.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
