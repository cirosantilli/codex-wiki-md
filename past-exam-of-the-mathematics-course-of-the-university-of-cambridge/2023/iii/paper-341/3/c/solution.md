<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Extend a grid vector $v$ by zero to the [Dirichlet boundary](../../../../../../dirichlet-boundary-condition.md). Pairing contributions along undirected nearest-neighbour edges gives the discrete energy identity

$$
\boxed{v^TAv=-\sum_{\{r,s\}\in E}(v_r-v_s)^2,}
$$

where $E$ includes edges from an interior node to a boundary node. This is the three-dimensional version of [summation by parts](../../../../../../abel-s-summation-formula.md) for the [seven-point Dirichlet Laplacian](../../../../../../seven-point-dirichlet-laplacian.md).

The right side is nonpositive. If it vanishes, every pair of neighbouring values agrees; connectivity of the grid and the zero boundary values then imply $v=0$. Thus $v^TAv<0$ for every nonzero $v$, so $A$ is [negative definite](../../../../../../negative-definite-matrix.md). In particular, zero is not an [eigenvalue](../../../../../../eigenvalue.md), and therefore

$$
\boxed{A\text{ is nonsingular}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
