<h1 id="section-f/47/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $z_{ij}$ be the input to output weight $w_j$ for datum $i$, including $z_{i0}=1$ for the bias. With identity output activation, $h_i=a_i=\sum_jw_jz_{ij}$. The [chain rule](../../../../../../chain-rule.md) gives

$$
\boxed{\frac{\partial E_i}{\partial w_j}=(h_i-y_i)z_{ij}}.
$$

The $z_{ij}$ are held fixed when differentiating an output-layer weight; they may be hidden-layer activations rather than raw descriptors. Hidden-weight derivatives require [backpropagation](../../../../../../backpropagation.md) through the preceding layers.

## ↑ Ancestors (14)

1. [A](../a.md)
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
