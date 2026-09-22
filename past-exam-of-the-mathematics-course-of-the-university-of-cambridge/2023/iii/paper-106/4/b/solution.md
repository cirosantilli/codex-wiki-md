<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The estimate

$$
|\mu_{x,y}(T)|=|\langle Tx,y\rangle|
\leq\|T\|\,\|x\|\,\|y\|
$$

shows $\|\mu_{x,y}\|\leq\|x\|\|y\|$. For nonzero $x,y$, the rank-one operator

$$
Tz=\left\langle z,\frac{x}{\|x\|}\right\rangle\frac{y}{\|y\|}
$$

has norm one and attains equality. The zero cases are immediate.

Embed the operator unit ball into

$$
\prod_{(x,y)\in H\times H}
[-\|x\|\|y\|,\|x\|\|y\|]
$$

by $T\mapsto(\langle Tx,y\rangle)_{x,y}$. The product is compact by [Tychonoff theorem](../../../../../../tychonoff-s-theorem.md). A pointwise limit of these coordinates is a bilinear form $\theta$ satisfying

$$
|\theta(x,y)|\leq\|x\|\|y\|.
$$

By the stated representation theorem for bounded bilinear forms, $\theta(x,y)=\langle Tx,y\rangle$ for a unique operator with $\|T\|\leq1$. The image is therefore closed and compact. Its product topology is precisely the [weak operator topology](../../../../../../weak-operator-topology.md) $\sigma(\mathcal B(H),M)$.

The linear span $Z=\operatorname{span}M$ separates operators, and the preceding compactness lets part (a) identify $\mathcal B(H)$ isometrically with $Z^*$. Thus $\mathcal B(H)$ is a dual Banach space. This is the [operator predual from matrix coefficients](../../../../../../operator-predual-from-matrix-coefficients.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
