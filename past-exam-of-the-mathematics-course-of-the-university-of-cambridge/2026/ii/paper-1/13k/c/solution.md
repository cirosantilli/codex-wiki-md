<h1 id="13k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [log-linear model](../../../../../../log-linear-model.md) fit1 has only three main effects, so its fitted mean factors into a species factor, a diameter factor, and a height factor: mutual independence. Fit2 adds the species-diameter interaction, allowing those variables to associate, while asserting $\text{Height}\perp(\text{Species},\text{Diameter})$.

The likelihood-ratio deviance drop $12.606$ on one degree of freedom has $p=0.0003845$, strong evidence against species-diameter independence. Test fit2's remaining independence claim by comparing it with a model adding both Species:Height and Diameter:Height interactions (equivalently compare fit2 with the saturated model); its residual deviance $12.431$ is assessed against $\chi^2_3$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13K](../../13k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
