<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

Let $R$ be an [orthogonal matrix](../../../../../orthogonal-matrix.md) describing a Cartesian change of coordinates, with transformed [vector](../../../../../vector.md) components $v_i'=R_{ia}v_a$ and $w_j'=R_{jb}w_b$. Their [outer product](../../../../../outer-product.md) transforms as

$$
T_{ij}'=v_i'w_j'=R_{ia}R_{jb}T_{ab},
$$

which is the transformation law of a second-order Cartesian [tensor](../../../../../tensor.md). Here “rank two” counts tensor indices, not the [rank of a matrix](../../../../../matrix-rank.md); a nonzero [outer product](../../../../../outer-product.md) has matrix rank one.

For an [isotropic second-rank tensor](../../../../../isotropic-second-rank-tensor.md), invariance means $RTR^T=T$ for every proper [rotation matrix](../../../../../rotation-matrix.md). The half-turn matrices $\operatorname{diag}(1,-1,-1)$, $\operatorname{diag}(-1,1,-1)$ and $\operatorname{diag}(-1,-1,1)$ force all off-diagonal entries to vanish. Quarter-turns around coordinate axes then force the three diagonal entries to be equal. Conversely $RIR^T=I$, so **the most general second-rank [isotropic tensor](../../../../../isotropic-tensor.md) is**

$$
\boxed{T_{ij}=\lambda\delta_{ij},\qquad\lambda\in\mathbb R.}
$$

Since $vw^T$ has matrix rank at most one, it cannot equal a nonzero scalar multiple of the three-dimensional identity. Thus its isotropy forces $vw^T=0$. If $v\ne0$, a nonzero component $v_i$ makes the entire $i$th row vanish only when $w=0$; the converse is immediate. **The required choices are exactly**

$$
\boxed{v=0\quad\text{or}\quad w=0.}
$$

For the [Levi-Civita symbol](../../../../../levi-civita-symbol.md), multilinearity and antisymmetry of the [determinant](../../../../../determinant.md) give

$$
R_{ia}R_{jb}R_{kc}\epsilon_{abc}=(\det R)\epsilon_{ijk}=\epsilon_{ijk}
$$

for every $R\in SO(3)$. This proves the [rotation invariance of the Levi-Civita symbol](../../../../../rotation-invariance-of-the-levi-civita-symbol.md), hence its third-rank isotropy. The convention is invariance under proper rotations: under an orthogonal reflection $\det R=-1$, the sign reverses. Thus it is a [pseudotensor](../../../../../pseudotensor.md) if transformations of both orientations are included.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
