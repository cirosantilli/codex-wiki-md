<h1 id="section-f/47/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $K$ mutually exclusive classes, the output layer should provide $K$ nonnegative [probabilities](../../../../../../probability.md) summing to one, with labels aligned consistently to output coordinates. A softmax activation on [logits](../../../../../../logit.md) $a_k$ provides

$$
\boxed{p_k=\frac{e^{a_k}}{\sum_{\ell=1}^K e^{a_\ell}}},\qquad \sum_kp_k=1.
$$

Subtracting $\max_\ell a_\ell$ from all [logits](../../../../../../logit.md) before exponentiation preserves these [probabilities](../../../../../../probability.md) and prevents numerical overflow. Categorical [cross-entropy](../../../../../../cross-entropy.md) $-\sum_ky_k\log p_k$ is appropriate for one-hot or probabilistic class targets. Independent sigmoid outputs fit a different setting in which multiple labels can be present simultaneously and their [probabilities](../../../../../../probability.md) need not sum to one.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [47](../../47.md)
3. [Section F](../../../section-f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
