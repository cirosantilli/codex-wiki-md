<h1 id="section-f/47/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Compose [affine maps](../../../../../../affine-map.md) with nonlinear hidden [activation functions](../../../../../../activation-function.md), for example $h(x)=W_2\operatorname{ReLU}(W_1x+b_1)+b_2$. Several hidden units can respond to different linear combinations of input features; later units combine their responses to represent curved or piecewise-linear decision boundaries and interactions. A product interaction can be understood from $xy=[(x+y)^2-(x-y)^2]/4$: units approximating nonlinear functions of $x+y$ and $x-y$ can represent effects that no single additive linear fit captures.

**Nonlinearity in hidden layers is essential:** with only identity activations, repeated [affine maps](../../../../../../affine-map.md) collapse to one [affine map](../../../../../../affine-map.md) regardless of depth. Width and depth determine available representations; [regularization](../../../../../../regularization.md), validation and suitable optimization are needed to learn useful rather than overfitted interactions. A nonlinear output activation alone applied to one linear score does not give an unrestricted model of [feature interactions](../../../../../../feature-interaction.md).

## ↑ Ancestors (14)

1. [D](../d.md)
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
