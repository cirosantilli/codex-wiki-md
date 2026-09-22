<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Add a sex-by-treatment [interaction term](../../../../../../interaction-term.md):

$$
\operatorname{logit}(p_i)=\beta_0+\beta_S M_i+\beta_TT_i+\beta_{ST}M_iT_i.
$$

In R the formula becomes `prop ~ sex * treatment`. There are four parameters for four cell probabilities, so this model is saturated and, provided the cell proportions lie strictly between zero and one, fits each observed proportion exactly. It therefore recovers all the stated order relations.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
