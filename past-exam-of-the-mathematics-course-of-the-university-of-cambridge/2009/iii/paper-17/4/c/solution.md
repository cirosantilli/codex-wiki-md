<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $\mathbf n$ to be the [unit normal](../../../../../../unit-normal.md), so $P(v)=v-\langle v,\mathbf n\rangle\mathbf n$ is [orthogonal projection](../../../../../../orthogonal-projection.md) onto $TM$. With $D$ the Euclidean [Levi-Civita connection](../../../../../../levi-civita-connection.md), the proposed derivative is

$$
\nabla_XY=P(D_{\widetilde X}\widetilde Y)|_M.
$$

It is a smooth tangent field, and independence of the extensions is given. Linearity follows from linearity of $D$ and $P$. Moreover, for $f\in C^\infty(M)$, take local extensions of $f,X,Y$ to obtain

$$
\nabla_{fX}Y=f\nabla_XY,\qquad \nabla_X(fY)=X(f)Y+f\nabla_XY,
$$

since $PY=Y$. Thus it is an [affine connection](../../../../../../affine-connection.md) on $M$.

For tangent fields $Y,Z$, the normal component of $DY$ pairs to zero with $Z$. Differentiating the ambient [inner product](../../../../../../inner-product.md) along $X$ gives

$$
Xg(Y,Z)=\langle D_XY,Z\rangle+\langle Y,D_XZ\rangle
=g(\nabla_XY,Z)+g(Y,\nabla_XZ).
$$

Hence it is a [metric connection](../../../../../../metric-connection.md) for the induced [Riemannian metric](../../../../../../riemannian-metric.md). The ambient torsion vanishes, so

$$
\nabla_XY-\nabla_YX=P(D_XY-D_YX)=P[X,Y]=[X,Y].
$$

Here the restriction of the ambient bracket is the intrinsic bracket and is tangent to $M$: [derivations](../../../../../../derivation-of-an-algebra.md) of functions restricted to $M$ give the same bracket, or this follows in submanifold coordinates. Thus the projected derivative is also a [torsion-free connection](../../../../../../torsion-free-connection.md). Uniqueness now proves

$$
\boxed{\nabla\text{ is the Levi-Civita connection of the induced metric.}}
$$

This is the [projected ambient connection](../../../../../../projected-ambient-connection.md). The projection formula requires a [unit normal](../../../../../../unit-normal.md). If a nonunit normal is used, its normal term must instead be $\langle DY,\mathbf n\rangle\mathbf n/\langle\mathbf n,\mathbf n\rangle$. For example, on the unit [circle](../../../../../../circle.md), taking $\mathbf n=2p$ and differentiating its unit tangent along itself gives $DY=-p$; the unnormalized printed expression would be $3p$, which is not tangent. Normalizing the normal removes that ambiguity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
