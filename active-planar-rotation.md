# Active planar rotation

↑ **Parent:** [Planar rotation](planar-rotation.md)

For column [coordinate vectors](coordinate-vector.md) in the fixed [Cartesian basis](cartesian-basis.md), an active [planar rotation](planar-rotation.md) sends $(x,y)^T$ to $(x\cos\theta-y\sin\theta,\,x\sin\theta+y\cos\theta)^T$. For $\theta=\pi/3$ [radians](radian.md),

$$
R_{\pi/3}=\begin{pmatrix}1/2&-\sqrt3/2\\\sqrt3/2&1/2\end{pmatrix},\qquad
R_{\pi/3}\begin{pmatrix}2\\0\end{pmatrix}=\begin{pmatrix}1\\\sqrt3\end{pmatrix}.
$$

The endpoint travels counterclockwise through $60^\circ$ along a [circle](circle.md) of radius $2$. Its [Euclidean norm](euclidean-norm.md) stays $\sqrt{1^2+(\sqrt3)^2}=2$. The second [Cartesian basis](cartesian-basis.md) direction becomes $R_{\pi/3}(0,1)^T=(-\sqrt3/2,1/2)^T$, whose [dot product](dot-product.md) with $(1,\sqrt3)^T$ is still zero.

<a id="image-an-active-counterclockwise-planar-rotation-by-pi-3-the-vector-moves-while-the-cartesian-basis-stays-fixed"></a>
![](rotation-counterclockwise-column-vector.png)

**[Figure 42](#image-an-active-counterclockwise-planar-rotation-by-pi-3-the-vector-moves-while-the-cartesian-basis-stays-fixed). An active counterclockwise planar rotation by $\pi/3$: the vector moves while the Cartesian basis stays fixed**.

A quick sign check is to look at the first column: $R_\theta(1,0)^T=(\cos\theta,\sin\theta)^T$ must point above the horizontal axis for $0<\theta<\pi$. The columns have unit [Euclidean norm](euclidean-norm.md) and zero [dot product](dot-product.md), so $R_\theta^TR_\theta=I$; the [determinant](determinant.md) is $\cos^2\theta+\sin^2\theta=1$. Finally, the [transpose](transpose.md) negates the off-diagonal entries, giving $R_\theta^T=R_{-\theta}$: turning back reverses the action. This is the same [matrix](matrix.md) used for [passive rotation of coordinates](passive-rotation-of-coordinates.md), though that interpretation keeps the [vector](vector.md) fixed.

## ↑ Ancestors (7)

1. [Planar rotation](planar-rotation.md)
2. [Rotation matrix](rotation-matrix.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Passive rotation of coordinates](passive-rotation-of-coordinates.md)
