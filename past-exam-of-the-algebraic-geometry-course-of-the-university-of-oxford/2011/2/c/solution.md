<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose projective embeddings $X\subseteq\mathbb P^n$ and $Y\subseteq\mathbb P^m$. Define their [product](../../../../product-of-numbers.md) as the Segre [image](../../../../image-of-a-function.md) of the [set](../../../../set-split.md) of pairs $(x,y)$, with its induced [variety](../../../../algebraic-variety-split.md) structure.

It is closed in the Segre [variety](../../../../algebraic-variety-split.md). To see this directly, for every homogeneous $f\in I(X)$ impose the equations $f(z_{0j},\ldots,z_{nj})=0$ on every column, and for every homogeneous $g\in I(Y)$ impose $g(z_{i0},\ldots,z_{im})=0$ on every row. For a [rank-one matrix](../../../../rank-one-matrix.md) $z_{ij}=x_iy_j$, the column equations are $y_j^{\deg f}f(x)=0$. A nonzero $y_j$ therefore forces $x\in X$. The row equations similarly force $y\in Y$. Thus these homogeneous equations together with the [minors](../../../../minor-linear-algebra.md) cut out exactly $X\times Y$, proving it is projective.

On a chart where $z_{i_0j_0}\neq0$, the projections have formulas

$$
\pi_X([Z])=[z_{0j_0}:\cdots:z_{nj_0}],\qquad
\pi_Y([Z])=[z_{i_00}:\cdots:z_{i_0m}].
$$

These [homogeneous coordinate](../../../../homogeneous-coordinate.md) tuples are nonzero on the chart and agree on overlaps, so both projections are [morphisms](../../../../morphism-of-algebraic-varieties.md).

Given [morphisms](../../../../morphism-of-algebraic-varieties.md) $\alpha:Z\to X$ and $\beta:Z\to Y$, define $\gamma(z)=\sigma_{n,m}(\alpha(z),\beta(z))$. Locally write their coordinates as $[a_0:\cdots:a_n]$ and $[b_0:\cdots:b_m]$. Then $\gamma$ has coordinates $[a_ib_j]$, which are regular with a nonzero coordinate near each [point](../../../../point-geometry.md). Hence $\gamma$ is a [morphism](../../../../morphism-of-algebraic-varieties.md) and

$$
\boxed{\pi_X\circ\gamma=\alpha,\qquad\pi_Y\circ\gamma=\beta.}
$$

The two projections determine the underlying pair uniquely, so this [morphism](../../../../morphism-of-algebraic-varieties.md) is unique. This is the [product](../../../../product-of-numbers.md) [universal property](../../../../universal-property.md), and it makes the construction independent up to canonical [isomorphism](../../../../isomorphism.md) of the chosen embeddings.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebraic Geometry course of the University of Oxford](../../../split.md)
5. [Algebraic Geometry course of the University of Oxford](../../../../algebraic-geometry-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
