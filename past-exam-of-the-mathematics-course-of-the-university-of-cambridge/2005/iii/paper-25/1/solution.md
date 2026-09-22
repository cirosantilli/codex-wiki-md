<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use tangent vectors, rather than the affine tangent plane, to differentiate. Every skew-symmetric [matrix](../../../../../matrix.md) $A$ gives a curve $X\exp(tA)$ in the [special orthogonal group](../../../../../special-orthogonal-group.md). Its first derivative under $f$ is $\operatorname{tr}(CXA)$. The trace pairing annihilates every skew-symmetric [matrix](../../../../../matrix.md) precisely when $CX$ is symmetric: choosing $A$ with only entries $a_{ij}=-a_{ji}$ tests each off-diagonal antisymmetric entry. Thus criticality is equivalent to $Y=CX$ being symmetric.

Since $X$ is orthogonal, $YY^T=C^2$, so at a [critical point](../../../../../critical-point.md) $Y^2=C^2$. Consequently $Y$ commutes with $C^2$. The diagonal entries $c_i^2$ are distinct, and the equation $YC^2=C^2Y$ gives $(c_j^2-c_i^2)y_{ij}=0$ for $i\ne j$. Hence $Y$ and $X$ are diagonal. Orthogonality and the determinant constraint give exactly

$$
\boxed{D=\operatorname{diag}(\varepsilon_1,\ldots,\varepsilon_n),\qquad\varepsilon_i\in\{1,-1\},\quad\prod_i\varepsilon_i=1.}
$$

Conversely each such $D$ makes $CD$ symmetric, so this list is complete.

To calculate the [Hessian matrix](../../../../../hessian-matrix.md), use local coordinates $X=\exp(A)D$ with $A^T=-A$; the [matrix exponential](../../../../../matrix-exponential.md) is a local coordinate map near zero. Its quadratic term gives

$$
\operatorname{Hess}_D f(A,A)=\operatorname{tr}(CA^2D)=-\sum_{i<j}(c_i\varepsilon_i+c_j\varepsilon_j)a_{ij}^2,
$$

because $(A^2)_{ii}=-\sum_{j\ne i}a_{ij}^2$. There are no mixed quadratic terms. For $i<j$, $c_j>c_i>0$, so $c_i\varepsilon_i+c_j\varepsilon_j$ has the sign of $\varepsilon_j$ and is never zero. Every listed [critical point](../../../../../critical-point.md) is therefore nondegenerate, with [Morse index](../../../../../morse-index.md)

$$
\boxed{\operatorname{ind}(D)=\#\{(i,j):i<j,\ \varepsilon_j=1\}=\sum_{j:\varepsilon_j=1}(j-1).}
$$

This is the [trace height on the special orthogonal group](../../../../../trace-height-on-the-special-orthogonal-group.md) calculation; the rotations in the hint select the individual coordinates $a_{ij}$.

For $n=3$, the signs $(+--),(-+-),(--+),(+++)$ have indices $0,1,2,3$ respectively. A [Morse function](../../../../../morse-function.md) on a compact closed [manifold](../../../../../topological-manifold.md) has [Euler characteristic](../../../../../euler-characteristic.md) equal to the alternating number of [critical points](../../../../../critical-point.md), by its [Morse handle-attachment theorem](../../../../../morse-handle-attachment-theorem.md) and resulting finite [CW complex](../../../../../cw-complex.md). Hence

$$
\boxed{\chi(SO(3))=1-1+1-1=0.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
