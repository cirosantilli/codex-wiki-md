<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [submersion](../../../../../../submersion.md) is a [smooth map between manifolds](../../../../../../smooth-map-between-manifolds.md) $F:X^n\to Y^m$ for which

$$
D_pF:T_pX\longrightarrow T_{F(p)}Y
$$

is surjective at every $p\in X$.

The local submersion theorem says that around every $p\in X$ there are coordinates $(x^1,\ldots,x^n)$ centered at $p$ and $(y^1,\ldots,y^m)$ centered at $F(p)$ in which

$$
F(x^1,\ldots,x^n)=(x^1,\ldots,x^m).
$$

To prove it, surjectivity lets us choose $m$ source coordinates such that $dF^1,\ldots,dF^m$ are independent. Complete them by source coordinates $x^{m+1},\ldots,x^n$ and define

$$
G=(F^1,\ldots,F^m,x^{m+1},\ldots,x^n).
$$

The derivative of $G$ is invertible at $p$, so the [inverse function theorem](../../../../../../inverse-function-theorem.md) makes $G$ a local coordinate system; in these coordinates $F$ is the displayed projection.

For $q\in Y$, the fiber is locally given by

$$
x^1=q^1,\ldots,x^m=q^m.
$$

These are slice coordinates, so $F^{-1}(q)$ is an [embedded submanifold](../../../../../../embedded-submanifold.md) of dimension $n-m$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
