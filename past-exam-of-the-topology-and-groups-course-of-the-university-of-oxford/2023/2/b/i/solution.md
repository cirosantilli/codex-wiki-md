<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $A=T^2\setminus B^2$ and let $E=\partial A=S^1$ denote the attaching [circle](../../../../../circle.md). The version of the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) used here states that if $X=U\cup V$ is an [open cover](../../../../../open-cover.md) with $U,V,U\cap V$ [path-connected](../../../../../path-connected-space.md) and a common [base point](../../../../../base-point.md) in $U\cap V$, then

$$
\pi_1(X)\cong\pi_1(U)*_{\pi_1(U\cap V)}\pi_1(V).
$$

The expression on the right means the [pushout of groups](../../../../../pushout-of-groups.md) of the two inclusion-induced [group homomorphisms](../../../../../group-homomorphism.md); they need not be [injective](../../../../../injective-function.md).

Choose a thin [collar neighbourhood](../../../../../collar-neighbourhood.md) $C_A$ of $E$ inside $A$, and a thin equatorial band $C_S$ inside $S^2$. For example, before the square's side identifications take $C_A=\{v:1\leq|v|<1+\epsilon\}$ with $0<\epsilon<1/2$, and take $C_S=\{(x,y,z)\in S^2:|z|<\epsilon\}$. In the glued [topological space](../../../../../topological-space.md) set

$$
U=A\cup C_S,\qquad V=S^2\cup C_A.
$$

These are [open subsets](../../../../../open-set.md): their preimages in the two pieces are open and respect the gluing. They cover $X$, and the three [deformation retractions](../../../../../deformation-retraction.md)

$$
U\simeq A,\qquad V\simeq S^2,\qquad U\cap V=C_A\cup_E C_S\simeq E
$$

fix $E$. Thus all three spaces are [path-connected](../../../../../path-connected-space.md), and a [base point](../../../../../base-point.md) $b\in E$ is preserved.

For completeness, the [fundamental group of a once-punctured torus](../../../../../fundamental-group-of-a-once-punctured-torus.md) is $F(a,b)$, and its [boundary loop of a once-punctured torus](../../../../../boundary-loop-of-a-once-punctured-torus.md) represents $[a,b]=aba^{-1}b^{-1}$, up to [orientation](../../../../../orientation-of-a-simplex.md) and a change of [base point](../../../../../base-point.md). Here is the geometry behind both facts. In the square model, move each point of $A$ radially outwards to the square boundary:

$$
v\longmapsto\left((1-t)+\frac{2t}{\max(|v_1|,|v_2|)}\right)v,\qquad 0\leq t\leq1.
$$

The denominator never vanishes on $A$. The [homotopy](../../../../../homotopy-split.md) stays outside the missing [open disk](../../../../../open-disk.md), stays inside the square, and fixes the square boundary, so it descends through the side identifications. The resulting [retract](../../../../../retract.md) is a [wedge of two circles](../../../../../wedge-of-two-circles.md). Its [fundamental group](../../../../../fundamental-group.md) is the [free group](../../../../../free-group.md) on the two oriented side [based loops](../../../../../based-loop.md) $a,b$. The inner [boundary loop](../../../../../boundary-loop.md) travels around the square once under this [deformation retraction](../../../../../deformation-retraction.md); its successive sides read $a,b,a^{-1},b^{-1}$.

The [sphere](../../../../../sphere.md) $S^2$ is [simply connected](../../../../../simply-connected-space.md). Hence the [group homomorphism](../../../../../group-homomorphism.md) from $\pi_1(E)\cong\mathbb Z$ to $\pi_1(V)$ is trivial, while its map to $\pi_1(U)$ sends a [group generator](../../../../../generator-of-a-group.md) to $[a,b]$. Applying the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) gives

$$
\boxed{\pi_1(X,b)\cong F(a,b)/\langle\!\langle[a,b]\rangle\!\rangle
=\langle a,b\mid aba^{-1}b^{-1}=1\rangle\cong\mathbb Z^2.}
$$

The final [group isomorphism](../../../../../group-isomorphism.md) follows because the single [relator](../../../../../relator.md) makes $a,b$ commute, leaving the [free abelian group](../../../../../free-abelian-group.md) on two [group generators](../../../../../generator-of-a-group.md). The two hemispheres kill the same [boundary loop](../../../../../boundary-loop.md); they do not create another [group generator](../../../../../generator-of-a-group.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology and groups course of the University of Oxford](../../../../split.md)
6. [Topology and groups course of the University of Oxford](../../../../../topology-and-groups-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
