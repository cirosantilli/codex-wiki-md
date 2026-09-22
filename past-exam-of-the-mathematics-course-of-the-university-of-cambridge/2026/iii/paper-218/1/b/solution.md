<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Writing $d_i$ for difficulty, model1 assumes independent responses

$$
Y_i\sim\operatorname{IG}(\mu_i,\lambda),
\qquad
\frac1{\mu_i^2}=\beta_0+\beta_1d_i,
$$

with common dispersion. The estimates are $\widehat\beta_0=9.0827$ and $\widehat\beta_1=-1.4323$.

One extra difficulty level decreases the fitted inverse squared mean response time by $1.4323$. Since $\mu=(\beta_0+\beta_1d)^{-1/2}$, this means that fitted mean response time increases with difficulty. The negative coefficient is therefore unsurprising; its sign looks counterintuitive only if the inverse-squared [link function](../../../../../../link-function.md) is ignored. The independence assumption is questionable because every subject contributes eight repeated responses.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
