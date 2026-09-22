<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

A positively oriented planar [rotation matrix](../../../../../rotation-matrix.md) acts by

$$
\boxed{\begin{pmatrix}x_1'\\x_2'\end{pmatrix}
=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}
\begin{pmatrix}x_1\\x_2\end{pmatrix}.}
$$

For a [unit vector](../../../../../unit-vector.md) $n$ in three dimensions, the parallel and perpendicular [orthogonal projections](../../../../../orthogonal-projection.md) are

$$
x_\parallel=(x\cdot n)n,\qquad x_\perp=x-(x\cdot n)n.
$$

On the plane perpendicular to $n$, the map $v\mapsto n\times v$ preserves lengths and turns vectors through a positive right angle about $n$. It squares to minus the identity there. Thus $\cos\theta\,x_\perp+\sin\theta(n\times x_\perp)$ rotates that component, while the parallel component remains fixed. This proves the [Rodrigues rotation formula](../../../../../rodrigues-rotation-formula.md)

$$
x'=(x\cdot n)n+\cos\theta\,[x-(x\cdot n)n]+\sin\theta(n\times x).
$$

Its component form uses the [Levi-Civita symbol](../../../../../levi-civita-symbol.md):

$$
\boxed{R_{ij}=\cos\theta\,\delta_{ij}+(1-\cos\theta)n_in_j-\sin\theta\,\epsilon_{ijk}n_k.}
$$

Since $n_in_i=1$ and $\epsilon_{iik}=0$, its [matrix trace](../../../../../matrix-trace.md) is $3\cos\theta+1-\cos\theta=1+2\cos\theta$.

For the given matrix, the [matrix trace](../../../../../matrix-trace.md) is $1+2r$ with $r=1/\sqrt2$, so $\cos\theta=1/\sqrt2$. In the stated angular range, $\theta=\pm\pi/4$. The antisymmetric entries give

$$
2\sin\theta\,n=(R_{32}-R_{23},R_{13}-R_{31},R_{21}-R_{12})=(1,1,0).
$$

Therefore the two axis-angle pairs are

$$
\boxed{\left(\frac\pi4,\frac{(1,1,0)}{\sqrt2}\right),\qquad
\left(-\frac\pi4,-\frac{(1,1,0)}{\sqrt2}\right).}
$$

Reversing the axis and the angle leaves the [Rodrigues rotation formula](../../../../../rodrigues-rotation-formula.md) unchanged, so these describe the same rotation.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
