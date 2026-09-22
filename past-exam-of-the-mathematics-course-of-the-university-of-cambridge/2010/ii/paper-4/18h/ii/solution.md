<h1 id="18h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The previous permutation calculation shows that every automorphism either preserves $x^3,y^3$ separately or interchanges them. Their sum and product are therefore fixed by the [Galois group](../../../../../../galois-group.md) and belong to $K$, proving the quadratic assertion.

For the depressed cubic, $\alpha+\beta+\gamma=0$, $\alpha\beta+\alpha\gamma+\beta\gamma=b$, and $\alpha\beta\gamma=-c$. Using $1+\zeta+\zeta^2=0$ gives

$$
x+y=3\alpha,\qquad xy=-3b,
$$

and hence

$$
x^3+y^3=(x+y)^3-3xy(x+y)
=27(\alpha^3+b\alpha)=-27c.
$$

Also $x^3y^3=-27b^3$. The desired [polynomial](../../../../../../polynomial-split.md) is

$$
\boxed{T^2+27cT-27b^3.}
$$

Its [discriminant](../../../../../../discriminant.md) is $729c^2+108b^3=-27D$, where $D=-4b^3-27c^2$. Here $-27$ is a square in $K$, since $[3(\zeta-\zeta^2)]^2=-27$.

One can justify the group criterion directly even when one resolvent vanishes. The nonzero root-difference product

$$
d=(\alpha-\beta)(\alpha-\gamma)(\beta-\gamma)
$$

has $d^2=D$ and changes sign exactly under odd root permutations. It is fixed by the entire group exactly when the group is contained in $A_3$. If $D$ is a square in $K$, then $d$ equals one of its two square roots in $K$; conversely, a fixed $d$ lies in $K$. Therefore

$$
\boxed{\operatorname{Gal}(F/K)=
\begin{cases}C_3,&D\in K^{\times2},\\S_3,&D\notin K^{\times2}.\end{cases}}
$$

Separability ensures $D\ne0$, and the characteristic hypotheses ensure that all divisions and the sign argument are valid.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
