# Passive rotation of coordinates

↑ **Parent:** [Rotation matrix](rotation-matrix.md)

Rotate an [orthonormal basis](orthonormal-basis.md) counterclockwise by $\theta$ while keeping the [vector](vector.md) $v$ fixed. The new [basis vectors](basis-vector.md), written in the old [basis](basis.md), are the columns of $P=R_\theta$. The [change-of-basis matrix](change-of-basis-matrix.md) convention therefore gives

$$
[v]_{\rm old}=R_\theta[v]_{\rm new},\qquad
[v]_{\rm new}=R_\theta^{-1}[v]_{\rm old}=R_\theta^T[v]_{\rm old}=R_{-\theta}[v]_{\rm old}.
$$

For example, the fixed [vector](vector.md) with old [coordinate vector](coordinate-vector.md) $(2,0)^T$ has new [coordinate vector](coordinate-vector.md) $(1,-\sqrt3)^T$ after the [basis](basis.md) turns by $\pi/3$ [radians](radian.md). Its negative second coordinate means that the arrow lies below the new first axis. By contrast, an [active planar rotation](active-planar-rotation.md) through that same [angle](angle.md) moves the arrow to old coordinates $(1,\sqrt3)^T$. The sign difference follows from which object moves. The passive component formulas are $x'=x\cos\theta+y\sin\theta$, $y'=-x\sin\theta+y\cos\theta$.[§20–1, equation (20.3) and the preceding paragraph: the angle relates coordinate axes, not rotating objects](the-feynman-lectures-on-physics-volume-i-by-richard-feynman-and-others/chapter-20-rotation-in-space.md)

If [coordinate vectors](coordinate-vector.md) are instead written as rows, transposing the active equation gives $(v')^T=v^TR_\theta^T$. Switching to rows changes the side and the [transpose](transpose.md); it does not by itself turn an active [planar rotation](planar-rotation.md) into [passive rotation of coordinates](passive-rotation-of-coordinates.md).

## ↑ Ancestors (6)

1. [Rotation matrix](rotation-matrix.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Active planar rotation](active-planar-rotation.md)
- [Passive rotation of coordinates](passive-rotation-of-coordinates.md)
- [Rotation matrix](rotation-matrix.md)
