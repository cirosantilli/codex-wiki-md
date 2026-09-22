<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [Matrix Lie group](../../../../../matrix-lie-group.md), $T_gG$ consists of derivatives $\gamma'(0)$ of differentiable curves in $G$ with $\gamma(0)=g$, viewed inside $M_n(\mathbb C)$ as a real vector space. At the identity, multiplying two such curves adds their derivatives, and reparametrizing a curve multiplies its derivative by any real scalar. Thus $L(G)=T_IG$ is a real vector subspace.

If $Y\in L(G)$ and $g\in G$, conjugating a curve with derivative $Y$ proves $gYg^{-1}\in L(G)$. Let $g(s)$ have $g(0)=I$ and $g'(0)=X\in L(G)$. Differentiating the curve $g(s)Yg(s)^{-1}$ inside the finite-dimensional, hence closed, vector subspace $L(G)$ gives

$$
XY-YX\in L(G).
$$

The matrix [commutator](../../../../../commutator.md) is real bilinear, antisymmetric, and satisfies the [Jacobi identity](../../../../../jacobi-identity.md) by associativity of matrix multiplication. This proves that **$L(G)$ is a real [Lie algebra](../../../../../lie-algebra-split.md)**.

The exponential-map theorem for a linear [Lie group](../../../../../lie-group.md) says $\exp X\in G$ whenever $X\in L(G)$. Applying it to every real multiple of $X$ gives $\exp(tX)\in G$ for every real $t$. Conversely that curve has derivative $X$ at zero, so $X\in L(G)$. Hence

$$
\boxed{X\in L(G)\iff\exp(tX)\in G\ \text{for every }t\in\mathbb R}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the lie Groups and Differentiable Manifolds course of the University of Oxford](../../../../split.md)
6. [Lie Groups and Differentiable Manifolds course of the University of Oxford](../../../../../lie-groups-and-differentiable-manifolds-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
