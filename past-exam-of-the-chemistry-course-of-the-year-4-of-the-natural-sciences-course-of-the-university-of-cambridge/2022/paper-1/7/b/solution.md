<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A weighting function must first be normalized to a [probability density](../../../../../probability-density.md). The constant choice on $[a,b]$ means

$$
q(x)=\frac1{b-a},\qquad
I=\mathbb E_q\left[\frac{f(X)}{q(X)}\right]=(b-a)\mathbb E_q[f(X)].
$$

Equivalently, transform $x=a+(b-a)z$ and use the already normalized $g(z)=1$ on $[0,1]$. Independent samples give the unbiased [Monte Carlo integration](../../../../../monte-carlo-integration.md) estimator

$$
\boxed{\widehat I_N=\frac{b-a}{N}\sum_{j=1}^N f(a+(b-a)U_j),\quad U_j\sim\mathrm{Uniform}(0,1).}
$$

```
function uniform_monte_carlo(f, a, b, N):
    require N >= 2
    total = 0
    total_squared = 0
    for j in 1,...,N:
        u = independent_uniform_0_1()
        value = f(a+(b-a)*u)
        total += value
        total_squared += value*value
    average = total/N
    sample_variance = (total_squared-N*average*average)/(N-1)
    integral = (b-a)*average
    standard_error = abs(b-a)*sqrt(sample_variance/N)
    return integral, standard_error
```

For a general positive normalized importance density $q$, replace each sample contribution by $f(X_j)/q(X_j)$ with $X_j\sim q$. Here the uniform choice is the special case of [importance sampling](../../../../../importance-sampling.md) that assigns equal weight to every region of equal length.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
