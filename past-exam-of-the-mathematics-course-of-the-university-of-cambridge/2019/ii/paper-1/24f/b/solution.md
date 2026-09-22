<h1 id="24f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Homogenizing the affine equation gives the [projective closure](../../../../../../projective-completion.md)

$$
C=\{[X:Y:Z]\in\mathbb P^2:
X^3Y+Y^3Z+Z^3X=0\}.
$$

This is the [Klein quartic](../../../../../../klein-quartic.md). It is smooth: if all three projective partial derivatives vanished, then

$$
3X^2Y=-Z^3,
\qquad
3Y^2Z=-X^3,
\qquad
3Z^2X=-Y^3.
$$

Multiplying them gives $28X^3Y^3Z^3=0$. If one coordinate is zero, the displayed equations force all three to vanish, which is impossible in projective space. Thus $C$ is a smooth compactification of $X'$. The smooth compactification compatible with the extended coordinate functions is its normalization, and since $C$ is already smooth it is biholomorphic to $C$.

For a direct genus computation, consider the extended coordinate map $\pi_x:X\to\mathbb C_\infty$. A generic $x$ leaves the cubic equation

$$
y^3+x^3y+x=0,
$$

so $\deg\pi_x=3$. In the affine part, ramification occurs where $F_y=0$. Solving $F=F_y=0$ gives $(0,0)$ and the seven points

$$
y^7=-\frac38,
\qquad
x=2y^3.
$$

At the origin, $x=-y^3+O(y^6)$, so the [ramification index of a holomorphic map](../../../../../../ramification-index-of-a-holomorphic-map.md) is three and the contribution is two. At each of the other seven points, $F_x=-7/2\ne0$, $F_y=0$, and $F_{yy}=6y\ne0$, so the ramification index is two and each contributes one.

There are two points at infinity. Near $P=[1:0:0]$, in coordinates $u=Y/X$, $v=Z/X$, the equation is

$$
u+u^3v+v^3=0,
$$

and $1/x=v$, so $P$ is unramified. Near $Q=[0:1:0]$, in coordinates $r=X/Y$, $s=Z/Y$, the equation is

$$
r^3+s+rs^3=0.
$$

Thus $s=-r^3+O(r^{10})$ and $1/x=s/r=-r^2+O(r^9)$, so $Q$ has ramification index two and contributes one. The total ramification is therefore

$$
2+7+1=10.
$$

The [Riemann-Hurwitz formula](../../../../../../riemann-hurwitz-formula.md) for the degree-three map to the sphere gives

$$
2g(X)-2=3(2\cdot0-2)+10=4,
$$

and hence

$$
\boxed{g(X)=3}.
$$

This also agrees with the [genus of a smooth plane curve](../../../../../../genus-of-a-smooth-plane-curve.md) of degree four.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [24F](../../24f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
