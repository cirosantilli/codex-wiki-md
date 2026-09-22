<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

Use the right-handed [rotation matrix](../../../../../rotation-matrix.md) which sends the positive $x$ direction to the positive $y$ direction:

$$
R=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&1\end{pmatrix}.
$$

The [Cartesian second-rank tensor](../../../../../cartesian-second-rank-tensor.md) transformation law gives

$$
S'=RSR^{\mathsf T}=\begin{pmatrix}
S_{22}&-S_{21}&-S_{23}\\
-S_{12}&S_{11}&S_{13}\\
-S_{32}&S_{31}&S_{33}
\end{pmatrix}.
$$

Here [isotropic tensor](../../../../../isotropic-tensor.md) means invariant under every proper [rotation](../../../../../rotation-mathematics.md), as is needed for the rank-three assertion involving the [Levi-Civita symbol](../../../../../levi-civita-symbol.md). A passive coordinate [rotation](../../../../../rotation-mathematics.md) through the same angle uses $R^{\mathsf T}$ instead; the invariance conclusions are identical.

Setting $S'=S$ forces $S_{11}=S_{22}$, $S_{12}=-S_{21}$, and $S_{13}=S_{23}=S_{31}=S_{32}=0$. No symmetry assumption on $S$ has been made: it now has the form

$$
S=\begin{pmatrix}a&b&0\\-b&a&0\\0&0&c\end{pmatrix}.
$$

Invariance under a right-handed quarter-turn about the $x$ axis next gives $S_{22}=S_{33}$ and $S_{12}=-S_{13}$, hence $a=c$ and $b=0$. Conversely $R(\lambda I)R^{\mathsf T}=\lambda I$ for every [orthogonal matrix](../../../../../orthogonal-matrix.md). The general [isotropic second-rank tensor](../../../../../isotropic-second-rank-tensor.md) is therefore **$S_{ij}=\lambda\delta_{ij}$**.

An isotropic [vector](../../../../../vector.md) must be fixed by the half-turn about the $z$ axis, so its first two components vanish. The half-turn about the $x$ axis then forces its third component to vanish. Thus **the only isotropic [vector](../../../../../vector.md) is zero**. The general [isotropic third-rank tensor](../../../../../isotropic-third-rank-tensor.md) under proper [rotations](../../../../../rotation-mathematics.md) is **$A_{ijk}=\lambda\epsilon_{ijk}$**. If invariance under the whole [orthogonal group](../../../../../orthogonal-group.md) were required of an ordinary rank-three [tensor](../../../../../tensor.md), inversion $R=-I$ would send $A$ to $-A$, forcing $A=0$ instead.

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
