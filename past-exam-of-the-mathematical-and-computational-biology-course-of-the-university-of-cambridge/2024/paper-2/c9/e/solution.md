<h1 id="c9/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Recompute the root conditional [likelihoods](../../../../../likelihood-function.md) at the fitted rate, then multiply by the uniform root prior and normalize. The factors $1/4$ cancel between numerator and denominator:

$$
p(a\mid\text{leaf data},\widehat\mu)
=\frac{L_{\mathrm{root}}(a)}{\sum_bL_{\mathrm{root}}(b)}.
$$

```
prob = initialise_prob(leaves)
felsenstein(prob, mu_max, len(leaves), left, right, left_time, right_time)
root_posterior = prob[-1] / prob[-1].sum()
print(dict(zip("ACGT", root_posterior)))
```

At the refined optimum, the [posterior distribution](../../../../../bayesian-posterior.md) is

$$
\boxed{(p_A,p_C,p_G,p_T)\simeq(0.115499,\ 0.152301,\ 0.616701,\ 0.115499).}
$$

Thus G is the most probable ancestral base, but it is not inferred with certainty. This conditions on the fitted rate and does not additionally average over uncertainty in that rate.

## ↑ Ancestors (13)

1. [E](../e.md)
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
