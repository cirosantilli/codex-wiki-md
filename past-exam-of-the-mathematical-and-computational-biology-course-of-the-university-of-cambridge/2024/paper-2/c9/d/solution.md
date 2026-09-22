<h1 id="c9/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Evaluate the [log-likelihood function](../../../../../log-likelihood.md) on the specified interval, retaining the rate with the largest value. A grid spacing of $0.001$ finds $0.157$; refining locally avoids relying on a coarse-grid location when reporting three significant figures:

```
def evaluate(mu):
    p = initialise_prob(leaves)
    return felsenstein(p, mu, len(leaves), left, right, left_time, right_time)

coarse = np.linspace(.1, 1., 901)
centre = coarse[np.argmax([evaluate(mu) for mu in coarse])]
fine = np.linspace(max(.1, centre-.001), min(1., centre+.001), 2001)
mu_max = float(fine[np.argmax([evaluate(mu) for mu in fine])])
print(f"mu = {mu_max:.3g}; log-likelihood = {evaluate(mu_max):.8f}")
```

**The maximum-likelihood estimate is $\boxed{\widehat\mu=0.157}$** to three significant figures, with refined value about $0.156556$ and log-likelihood $-9.86147978$. Under the alternative per-replacement convention this same fitted [transition matrix](../../../../../stochastic-matrix.md) has $\widehat q=\widehat\mu/3\simeq0.0521854$; these are equivalent parameterizations, not competing fitted trees.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [C9](../../c9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
