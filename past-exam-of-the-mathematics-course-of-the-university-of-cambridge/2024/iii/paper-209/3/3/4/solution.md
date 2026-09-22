<h1 id="3/3/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Reveal the field in the order $x_1,\ldots,x_K$ and evaluate its joint density at zero. By the [Spatial Markov property of the Gaussian free field](../../../../../../../spatial-markov-property-of-the-gaussian-free-field.md), after the values on

$$
R_i=\{a,x_1,\ldots,x_{i-1}\}
$$

have been fixed to zero, the remaining field is the GFF killed on $R_i$. Part 3 therefore gives

$$
\operatorname{Var}(\Gamma(x_i)\mid\Gamma(x_1)=\cdots=\Gamma(x_{i-1})=0)
=\frac12G_{R_i}(x_i,x_i).
$$

Factoring the joint density into [conditional probability](../../../../../../../conditional-probability.md) densities now yields

$$
p_\Gamma(0,\ldots,0)
=\prod_{i=1}^K
\frac1{\sqrt{\pi G_{R_i}(x_i,x_i)}}.
$$

The left side is intrinsic and does not depend on the order used to factor the density. Therefore

$$
\prod_{i=1}^KG_{R_i}(x_i,x_i)
$$

is independent of the ordering.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 209](../../../../paper-209-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
