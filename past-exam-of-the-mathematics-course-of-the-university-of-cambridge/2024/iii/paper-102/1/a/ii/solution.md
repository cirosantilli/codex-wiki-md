<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The one-dimensional quotient $V/W$ is trivial because every one-dimensional representation vanishes on the [derived algebra](../../../../../../../derived-series-of-a-lie-algebra.md) $[\mathfrak{sl}_2,\mathfrak{sl}_2]=\mathfrak{sl}_2$. Choose $v\in V$ mapping to $1\in V/W$. Then

$$
c(x)=xv\in W
$$

is a $1$-cocycle:

$$
c([x,y])=x,c(y)-y,c(x).
$$

We show that it is a coboundary.

Decompose $W$ into generalized eigenspaces of its [Casimir element](../../../../../../../casimir-element.md) $\Omega$. These are subrepresentations because $\Omega$ is central. On a generalized eigenspace with nonzero eigenvalue, $\Omega$ is invertible. If $(x_i)$ and $(x^i)$ are dual bases of $\mathfrak{sl}_2$ for the [Killing form](../../../../../../../killing-form.md), put

$$
u=\sum_i x_i c(x^i).
$$

Invariance of the Killing form and the cocycle identity give the standard Casimir calculation

$$
x u=\Omega c(x).
$$

Thus on every nonzero generalized eigenspace, $c(x)=x(\Omega^{-1}u)$.

On the zero generalized eigenspace, every irreducible composition factor has zero Casimir eigenvalue. By part i and the [classification of finite-dimensional sl2 representations](../../../../../../../classification-of-finite-dimensional-sl2-representations.md), each such factor is trivial. In a basis adapted to a composition series, the image of $\mathfrak{sl}_2$ is therefore strictly upper triangular and hence solvable. Since $\mathfrak{sl}_2$ is simple and non-solvable, that image is zero. The cocycle then vanishes because it kills $[\mathfrak{sl}_2,\mathfrak{sl}_2]$.

Combining the generalized eigenspaces gives $w\in W$ such that $c(x)=xw$ for every $x$. Hence $v-w$ is invariant, and

$$
V=W\oplus\mathbb C(v-w)
$$

is a decomposition into subrepresentations. This proves the codimension-one case of the [Weyl complete reducibility theorem](../../../../../../../weyl-complete-reducibility-theorem.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 102](../../../../paper-102-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
