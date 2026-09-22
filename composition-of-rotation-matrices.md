# Composition of rotation matrices

↑ **Parent:** [Rotation matrix](rotation-matrix.md)

Apply $R_1$ to a column [coordinate vector](coordinate-vector.md), then apply $R_2$ in the same fixed [basis](basis.md). The [function composition](function-composition.md) is

$$
v''=R_2(R_1v)=(R_2R_1)v.
$$

Thus the rightmost [matrix](matrix.md) acts first. The product is again a [rotation matrix](rotation-matrix.md), since $(R_2R_1)^T(R_2R_1)=I$ and $\det(R_2R_1)=1$. For [planar rotations](planar-rotation.md) about the same origin, the [sine addition formula](sine-addition-formula.md) and [cosine addition formula](cosine-addition-formula.md) give

$$
R_\beta R_\alpha=R_{\alpha+\beta}=R_\alpha R_\beta.
$$

For a concrete [composition of rotation matrices](composition-of-rotation-matrices.md), first rotate $(2,0)^T$ by $\pi/3$ [radians](radian.md), reaching $(1,\sqrt3)^T$, then by $\pi/6$ [radians](radian.md):

$$
\begin{pmatrix}\sqrt3/2&-1/2\\1/2&\sqrt3/2\end{pmatrix}
\begin{pmatrix}1\\\sqrt3\end{pmatrix}
=\begin{pmatrix}0\\2\end{pmatrix}.
$$

The total [angle](angle.md) is $\pi/2$. Reversing these two [planar rotations](planar-rotation.md) gives the same answer, but [noncommuting rotations about fixed axes](noncommuting-rotations-about-fixed-axes.md) show why one cannot assume that property for [rotations in three dimensions](rotation-in-three-dimensions.md).[Modern Robotics, §3.2.1.1, propositions 3.4–3.5, preprint p. 69: closure and the distinction between planar and spatial composition](modern-robotics-mechanics-planning-and-control-by-kevin-m-lynch-and-frank-c-park.md)

**Table of contents**

- [Noncommuting rotations about fixed axes](noncommuting-rotations-about-fixed-axes.md)

## ↑ Ancestors (6)

1. [Rotation matrix](rotation-matrix.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Composition of rotation matrices](composition-of-rotation-matrices.md)
