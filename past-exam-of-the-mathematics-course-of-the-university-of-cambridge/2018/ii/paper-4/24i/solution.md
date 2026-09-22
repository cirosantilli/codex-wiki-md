<h1 id="24i/solution">Solution</h1>

↑ **Parent:** [24I](../24i.md)

Let $H$ denote a [hyperplane-section divisor of a projective plane curve](../../../../../hyperplane-section-divisor-of-a-projective-plane-curve.md). The [adjunction formula](../../../../../adjunction-formula.md) for a smooth degree-$d$ [projective plane curve](../../../../../projective-plane-curve.md) states

$$
K_C\sim(d-3)H|_C.
$$

Since $\deg(H|_C)=d$, this gives the [canonical degree of a smooth plane curve](../../../../../canonical-degree-of-a-smooth-plane-curve.md)

$$
\boxed{\deg K_C=d(d-3)}.
$$

Combining this with $\deg K_C=2g-2$ gives the [genus of a smooth plane curve](../../../../../genus-of-a-smooth-plane-curve.md)

$$
\boxed{g(C)=\frac{(d-1)(d-2)}2}.
$$

[Homogenization](../../../../../homogenization-algebra.md) of the affine equation gives the [projective completion](../../../../../projective-completion.md)

$$
C=V(F)\subset\mathbb P^2,
\qquad
F(X,Y,Z)=X^3Z+XY^3+YZ^3.
$$

This is the [plane model y plus x cubed plus xy cubed equals zero of the Klein quartic](../../../../../plane-model-y-plus-x-cubed-plus-xy-cubed-equals-zero-of-the-klein-quartic.md): after the coordinate relabelling $[A:B:C]=[Y:X:Z]$, its equation is $A^3B+B^3C+C^3A=0$.

Its first partial derivatives are

$$
F_X=3X^2Z+Y^3,
\qquad
F_Y=3XY^2+Z^3,
\qquad
F_Z=X^3+3YZ^2.
$$

If one of $X,Y,Z$ vanishes at a common zero of these three derivatives, the displayed equations successively force all three coordinates to vanish, which is impossible in [projective space](../../../../../projective-space-split.md). If $XYZ\ne0$, multiplying the three derivative equations gives

$$
X^3Y^3Z^3=-27X^3Y^3Z^3,
$$

again a contradiction. The [Jacobian criterion](../../../../../jacobian-criterion.md) therefore proves that **$C$ is smooth**.

The rational function $y=Y/Z$ defines a [rational map of projective varieties](../../../../../rational-map-of-projective-varieties.md) $C\dashrightarrow\mathbb P^1$. Because $C$ is a [smooth projective curve](../../../../../smooth-projective-curve.md), it extends uniquely to a morphism

$$
\pi:C\longrightarrow\mathbb P^1.
$$

For a generic finite value of $y$, its fibre is given by the cubic

$$
x^3+y^3x+y=0,
$$

so the [degree of a holomorphic map](../../../../../degree-of-a-holomorphic-map.md) is $3$. The [discriminant of a depressed cubic](../../../../../discriminant-of-a-depressed-cubic.md) is

$$
\Delta(y)=-4y^9-27y^2=-y^2(4y^7+27).
$$

At $y=0$ the fibre consists of $(0,0)$. Since $F_y(0,0)=1$, the [holomorphic implicit function theorem](../../../../../holomorphic-implicit-function-theorem.md) gives

$$
y=-x^3+O(x^{10}),
$$

so $x$ is a [local coordinate](../../../../../local-coordinate.md) and $\pi$ has [ramification index of a holomorphic map](../../../../../ramification-index-of-a-holomorphic-map.md) $3$ there. Each of the seven distinct roots of $4y^7+27$ gives one double, but not triple, root of the cubic in $x$, hence seven further ramification points of index $2$.

It remains to inspect the points at infinity. They are

$$
P=[1:0:0],
\qquad
Q=[0:1:0].
$$

Near $Q$, set $u=X/Y$ and $v=Z/Y$. The equation becomes $u^3v+u+v^3=0$, so $u=-v^3+O(v^{10})$, while $y=1/v$ has a [simple pole](../../../../../simple-pole.md). Thus $e_Q=1$. Near $P$, set $s=Y/X$ and $t=Z/X$. Now $t+s^3+st^3=0$, so $t=-s^3+O(s^{10})$ and

$$
y=\frac{s}{t}=-s^{-2}(1+O(s^7)).
$$

Thus $y$ has a [double pole](../../../../../double-pole.md) at $P$ and $e_P=2$. These calculations are the [ramification of the x-coordinate on the Klein quartic](../../../../../ramification-of-the-x-coordinate-on-the-klein-quartic.md) after the coordinate relabelling above.

The total ramification contribution is

$$
(3-1)+7(2-1)+(2-1)=10.
$$

The [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) for the degree-three map to the [projective line](../../../../../projective-line.md) now gives

$$
2g(C)-2=3(-2)+10=4,
$$

and therefore

$$
\boxed{g(C)=3}.
$$

## ↑ Ancestors (10)

1. [24I](../24i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
