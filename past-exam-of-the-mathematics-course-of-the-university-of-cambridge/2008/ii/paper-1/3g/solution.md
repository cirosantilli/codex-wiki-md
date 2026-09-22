<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

Let $T$ be an [isometry](../../../../../isometry.md), and set $S(x)=T(x)-T(0)$. Then $S(0)=0$, and preservation of distances gives $|S(x)|=|x|$. The [polarization identity](../../../../../polarization-identity.md) yields

$$
\langle S(x),S(y)\rangle=\frac12\bigl(|S(x)|^2+|S(y)|^2-|S(x)-S(y)|^2\bigr)=\langle x,y\rangle.
$$

For a standard [orthonormal basis](../../../../../orthonormal-basis.md) $e_1,e_2,e_3$, put $v_i=S(e_i)$. These three vectors are an [orthonormal basis](../../../../../orthonormal-basis.md). Since $\langle S(x),v_i\rangle=x_i$, we have $S(x)=\sum_i x_iv_i=Qx$ for an [orthogonal matrix](../../../../../orthogonal-matrix.md) $Q$. Thus

$$
\boxed{T(x)=Qx+b,\qquad Q^TQ=I,\quad b=T(0),}
$$

an [affine map](../../../../../affine-map.md).

For a finite [isometry group](../../../../../isometry-group.md) $G$, take $c=|G|^{-1}\sum_{g\in G}g(0)$. An affine map preserves an affine average, so for any $h\in G$,

$$
h(c)=\frac1{|G|}\sum_{g\in G}h(g(0))=\frac1{|G|}\sum_{g\in G}g(0)=c.
$$

**The orbit barycentre is a common [fixed point](../../../../../fixed-point.md).** This proves the [fixed point of a finite Euclidean isometry group](../../../../../fixed-point-of-a-finite-euclidean-isometry-group.md) result.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
