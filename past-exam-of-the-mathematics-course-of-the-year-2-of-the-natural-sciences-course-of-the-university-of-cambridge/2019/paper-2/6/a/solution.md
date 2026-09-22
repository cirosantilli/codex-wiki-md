<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An order-$n$ Cartesian [tensor](../../../../../tensor.md) has $3^n$ components whose values in two orthonormal Cartesian frames satisfy

$$
T'_{i_1\ldots i_n}=R_{i_1j_1}\cdots R_{i_nj_n}T_{j_1\ldots j_n},\qquad R^TR=I,
$$

with repeated indices summed as in [Einstein notation](../../../../../einstein-notation.md). It is an [isotropic tensor](../../../../../isotropic-tensor.md) when its components are unchanged by every proper [rotation](../../../../../rotation-mathematics.md), $R\in SO(3)$.

For rank two, a half-turn about any coordinate axis changes the sign of each component having exactly one index along that axis. Invariance therefore makes every off-diagonal component zero. Quarter-turns interchanging two coordinate axes then require $T_{11}=T_{22}=T_{33}$. Thus, without assuming symmetry in advance,

$$
\boxed{T_{ij}=a\delta_{ij}}.
$$

Conversely, the [Kronecker delta](../../../../../kronecker-delta.md) is invariant because $R_{ik}R_{jk}=\delta_{ij}$, so every tensor of this form is isotropic.

For rank three the general proper-rotation invariant form is

$$
\boxed{T_{ijk}=b\epsilon_{ijk}},
$$

where $\epsilon_{ijk}$ is the [Levi-Civita symbol](../../../../../levi-civita-symbol.md). The convention matters: the [isotropic rank-three tensor and reflections](../../../../../isotropic-rank-three-tensor-and-reflections.md) distinction says that invariance of a polar [tensor](../../../../../tensor.md) under all $R\in O(3)$ would force $b=0$. A nonzero $\epsilon_{ijk}$ is invariant under proper [rotations](../../../../../rotation-mathematics.md), and is a [pseudotensor](../../../../../pseudotensor.md) under the full orthogonal group. The shell integrals below are invariant under reflections as well, so their odd moments vanish.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
