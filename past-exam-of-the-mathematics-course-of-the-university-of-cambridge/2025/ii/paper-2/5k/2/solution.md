<h1 id="5k/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

No dominance says that mean yield is affine in the number of $A$ alleles:

$$
\mu_{aa}=\alpha,
\qquad
\mu_{Aa}=\alpha+\delta,
\qquad
\mu_{AA}=\alpha+2\delta.
$$

Equivalently, $2\mu_{Aa}=\mu_{aa}+\mu_{AA}$. Fit that reduced model and compare it with Model 1 using

```
r
model3 <- lm(yield ~ count, data = potato)
anova(model3, model1)
```

The resulting one-degree-of-freedom F-test tests the no-dominance constraint against unrestricted genotype means.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5K](../../5k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
