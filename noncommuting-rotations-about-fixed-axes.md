# Noncommuting rotations about fixed axes

↑ **Parent:** [Composition of rotation matrices](composition-of-rotation-matrices.md)

Use a fixed right-handed [Cartesian basis](cartesian-basis.md) in three dimensions and active [rotations in three dimensions](rotation-in-three-dimensions.md) through $\pi/2$ [radians](radian.md). The [right-hand rule](right-hand-rule.md) gives the following [rotation matrices](rotation-matrix.md) about the positive $x$ and $z$ axes:

$$
R_x=\begin{pmatrix}1&0&0\\0&0&-1\\0&1&0\end{pmatrix},\qquad
R_z=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&1\end{pmatrix}.
$$

For the [vector](vector.md) $v=(1,1,0)^T$, the two orders give

$$
\begin{aligned}
v&\xrightarrow{R_x}(1,0,1)^T\xrightarrow{R_z}(0,1,1)^T,\\
v&\xrightarrow{R_z}(-1,1,0)^T\xrightarrow{R_x}(-1,0,1)^T.
\end{aligned}
$$

Both outputs have [Euclidean norm](euclidean-norm.md) $\sqrt2$, but they point in different directions. Each arrow below is a [vector](vector.md) from the origin; the curved paths track its endpoint during each [rotation in three dimensions](rotation-in-three-dimensions.md).

<a id="image-active-rotations-in-three-dimensions-about-fixed-axes-the-order-changes-the-final-vector"></a>
![](rotation-fixed-axes-noncommuting-composition.png)

**[Figure 41](#image-active-rotations-in-three-dimensions-about-fixed-axes-the-order-changes-the-final-vector). Active rotations in three dimensions about fixed axes: the order changes the final vector**.

The axes in this example remain fixed throughout. A command to turn about an object's own current axis describes a different operation because that axis can move after the first turn. With an object's [orthonormal basis](orthonormal-basis.md) represented by columns of $Q$, a fixed-axis [rotation matrix](rotation-matrix.md) $R$ acts by $RQ$, whereas the corresponding rotation expressed in the object's own [basis](basis.md) acts by $QR$.[Modern Robotics, §3.2.1.2, preprint pp. 72–73: premultiplication uses fixed-frame axes; postmultiplication uses body-frame axes](modern-robotics-mechanics-planning-and-control-by-kevin-m-lynch-and-frank-c-park.md)

## ↑ Ancestors (7)

1. [Composition of rotation matrices](composition-of-rotation-matrices.md)
2. [Rotation matrix](rotation-matrix.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Composition of rotation matrices](composition-of-rotation-matrices.md)
