<h1 id="8a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Preserving the Euclidean [scalar product](../../../../../../dot-product.md) means $(Ax)^T(Ay)=x^Ty$ for every pair of real [vectors](../../../../../../vector.md) $x,y$. Since these bilinear expressions agree on all pairs of [basis](../../../../../../basis.md) [vectors](../../../../../../vector.md), this is equivalent to $A^TA=I$: the columns of $A$ form an [orthonormal basis](../../../../../../orthonormal-basis.md).

The first column is a [unit vector](../../../../../../unit-vector.md), so it is $(\cos\theta,\sin\theta)^T$ for some real $\theta$. A perpendicular [unit vector](../../../../../../unit-vector.md) is one of the two choices $\varepsilon(-\sin\theta,\cos\theta)^T$, where $\varepsilon\in\{1,-1\}$. Hence **all the required [orthogonal matrices](../../../../../../orthogonal-matrix.md) are**

$$
\boxed{A=R(\theta)D_\varepsilon=\begin{pmatrix}\cos\theta&-\varepsilon\sin\theta\\\sin\theta&\varepsilon\cos\theta\end{pmatrix},\quad D_\varepsilon=\operatorname{diag}(1,\varepsilon),\quad\theta\in\mathbb R.}
$$

Here $R(\theta)$ is a [planar rotation](../../../../../../planar-rotation.md), and $\theta$ is determined modulo $2\pi$. To check the [group](../../../../../../group-split.md) laws explicitly, $D_\varepsilon R(\phi)=R(\varepsilon\phi)D_\varepsilon$, so

$$
(R(\theta)D_\varepsilon)(R(\phi)D_\eta)=R(\theta+\varepsilon\phi)D_{\varepsilon\eta}.
$$

This proves closure. The identity is $R(0)D_1=I$, the inverse of $R(\theta)D_\varepsilon$ is $R(-\varepsilon\theta)D_\varepsilon$, and associativity is inherited from [matrix multiplication](../../../../../../matrix-multiplication.md). Thus the set is the [orthogonal group](../../../../../../orthogonal-group.md) $O(2)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8A](../../8a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
