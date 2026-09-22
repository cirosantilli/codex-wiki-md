<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At $P_1$ the tangent slope is zero. The [elliptic-curve addition formula](../../../../../../elliptic-curve-addition-formula.md) gives

$$
\boxed{2P_1=(0,-15)=-P_1.}
$$

The chord from $P_1$ to $P_2$ has slope $(-3-15)/(-6)=3$, so its sum has $x$-coordinate $3^2-0-(-6)=15$ and $y$-coordinate $3(0-15)-15=-60$. Thus **$P_1+P_2=(15,-60)$**.

Reduction at the good prime seven gives $\widetilde E:y^2=x^3+1$. For $x=0,1,2,3,4,5,6$, the right sides are respectively $1,2,2,0,2,0,0$. There are respectively $2,2,2,1,2,1,1$ choices of $y$. Including the point at infinity gives **$\#\widetilde E(\mathbb F_7)=12$**. Its nonzero [torsion points of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md) of order two are $(3,0),(5,0),(6,0)$, so it cannot be cyclic. Its two-primary component is $(\mathbb Z/2\mathbb Z)^2$ and its three-primary component is cyclic of order three; hence

$$
\boxed{\widetilde E(\mathbb F_7)\cong\mathbb Z/2\mathbb Z\times\mathbb Z/6\mathbb Z.}
$$

In particular its exponent is six.

The [reduction of an elliptic curve](../../../../../../reduction-of-an-elliptic-curve.md) is a [group homomorphism](../../../../../../group-homomorphism.md) defined on every $\mathbb Q_7$-point by projectivity. Thus $6P$ reduces to the identity for every rational $P$. A finite point with integral coordinates reduces to an affine point, whose projective last coordinate is one, so it cannot reduce to the identity at infinity. Therefore **every nonzero finite point $6P$ has nonintegral coordinates**. If $6P=O$, it has no affine coordinates at all. This is the [reduction exponent obstruction to integral multiples](../../../../../../reduction-exponent-obstruction-to-integral-multiples.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
