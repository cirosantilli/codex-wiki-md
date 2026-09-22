<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat $X\geq0$ as a prescribed input [protein](../../../../../protein-split.md) [concentration](../../../../../concentration.md), and $Y(t),Z(t)\geq0$ as the downstream gene-product [concentrations](../../../../../concentration.md). Define the [Hill activation function](../../../../../hill-activation-function.md)

$$
h(u;K,n)=\frac{u^n}{K^n+u^n},\qquad K>0,\quad n>0.
$$

A minimal model with no basal expression is

$$
\boxed{\frac{dY}{dt}=a_Yh(X;K_{XY},n_{XY})-Y,\qquad
\frac{dZ}{dt}=a_Zh(X;K_{XZ},n_{XZ})-Z}.
$$

Here $a_Y,a_Z>0$ are maximal production rates, $K_{XY},K_{XZ}$ are [Hill constants](../../../../../hill-constant.md) with the same units as $X$, and $n_{XY},n_{XZ}$ are dimensionless [Hill coefficients](../../../../../hill-coefficient.md). The negative terms describe a [first-order reaction](../../../../../first-order-reaction.md) for loss of each gene product, with both rate constants set to one in the chosen time units. Thus $a_Y,a_Z$ have units of [concentration](../../../../../concentration.md) per time and the unit loss rates have units of inverse time.

The equations model [regulation of gene expression](../../../../../regulation-of-gene-expression.md) at the level of its effective [protein](../../../../../protein-split.md) output, without separate [messenger RNA](../../../../../messenger-rna.md) dynamics. The independent branches mean that neither $Y$ nor $Z$ regulates the other in this initial model. Additive basal production could be included, but is not required by the question and is set to zero throughout this example.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
