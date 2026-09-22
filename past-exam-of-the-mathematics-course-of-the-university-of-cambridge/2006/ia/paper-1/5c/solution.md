<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

For $y\ne0$, the squared [Euclidean norm](../../../../../euclidean-norm.md) of the [orthogonal projection](../../../../../orthogonal-projection.md) residual is nonnegative:

$$
0\le\left|x-\frac{x\cdot y}{|y|^2}y\right|^2
=|x|^2-\frac{(x\cdot y)^2}{|y|^2}.
$$

This proves the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) $|x\cdot y|\le|x||y|$. Equality holds exactly when $x$ is a scalar multiple of $y$. If $y=0$, equality is automatic. Equivalently, equality means the two vectors are [linearly dependent](../../../../../linear-dependence.md), including the cases with a zero vector.

For a point $C$ equidistant from the coordinate vertices,

$$
|C-e_i|^2=|C|^2-2C_i+1
$$

must be independent of $i$. Thus all $C_i$ are equal, and their sum is one. The [centroid](../../../../../centroid.md) is therefore

$$
\boxed{C=\frac1n(1,\ldots,1),\qquad |OC|=\frac1{\sqrt n}.}
$$

For every $x$ in the base [probability simplex](../../../../../probability-simplex.md), the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $1=(1,\ldots,1)\cdot x\le\sqrt n\,|x|$. Equality forces the same coordinates as $C$. Thus $C$ is the unique [closest point of a probability simplex to the origin](../../../../../closest-point-of-a-probability-simplex-to-the-origin.md).

The angle $\alpha$ between $OC$ and any edge from the origin to $e_i$ satisfies

$$
\cos\alpha=\frac{C\cdot e_i}{|C|\,|e_i|}=\frac1{\sqrt n}.
$$

Consequently

$$
\boxed{\alpha=\arccos(n^{-1/2})\longrightarrow\frac\pi2,\qquad |OC|\longrightarrow0.}
$$

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
