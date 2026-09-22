<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For ordered simplicial cochains, define the Alexander-Whitney [cup product](../../../../cup-product.md) by

$$
(\phi\smile\psi)[v_0,\ldots,v_{i+j}]
=\phi[v_0,\ldots,v_i]\,\psi[v_i,\ldots,v_{i+j}],
$$

using the front and back faces of each characteristic [simplex](../../../../simplex.md). Write $\delta$ for the [coboundary](../../../../coboundary.md), $\delta\phi=\phi\partial$. Expanding the face-boundary formula gives the graded Leibniz identity

$$
\delta(\phi\smile\psi)=\delta\phi\smile\psi+(-1)^i\phi\smile\delta\psi.
$$

In this expansion, face omissions on the front and back portions supply the two displayed terms, and their extra terms at the shared vertex cancel with opposite signs. Hence the cup of cocycles is a [cocycle](../../../../cocycle.md). If $\phi$ changes by $\delta a$, its product with a [cocycle](../../../../cocycle.md) changes by $\delta(a\smile\psi)$; changing $\psi$ by $\delta b$ changes it by $(-1)^i\delta(\phi\smile b)$. The product therefore descends to [cohomology](../../../../cohomology-split.md). It is associative by the three consecutive-face formula and has the constant degree-zero [cochain](../../../../singular-cochain.md) as unit.

In the wedge, every positive-dimensional [simplex](../../../../simplex.md) belongs to exactly one factor. Restricting positive-degree cochains therefore gives a direct sum of the two [cochain](../../../../singular-cochain.md) groups and splits the coboundaries in degrees above one. In degree one, the same splitting of coboundaries holds: any pair of degree-zero cochains on the factors can have their values at the glued vertices made equal by adding a constant to one factor, which does not change its [coboundary](../../../../coboundary.md). Thus restriction induces

$$
\boxed{H^n(X\vee Y)\cong H^n(X)\oplus H^n(Y)\quad(n>0)}.
$$

Represent classes from the two factors by cochains extended by zero on the other factor. If both degrees are positive, a [simplex](../../../../simplex.md) lies wholly in one factor, so one of the front or back evaluations is zero. Their [cup product](../../../../cup-product.md) is already zero as a [cochain](../../../../singular-cochain.md). This proves all the stated mixed products vanish.

For the indicated wedge there is one unit in degree zero, two generators $a,b$ in degree one, and one generator $c$ in degree two; higher groups vanish. Every product of positive-degree elements is zero. Its ring is therefore

$$
\boxed{\mathbb Z\oplus(\mathbb Za\oplus\mathbb Zb\oplus\mathbb Zc),\qquad |a|=|b|=1,\ |c|=2,\quad(a,b,c)^2=0}.
$$

The [torus](../../../../torus.md) has the same additive groups, but its degree-one generators have nonzero [cup product](../../../../cup-product.md) generating degree two. The two graded rings are not isomorphic. Since a [homotopy equivalence](../../../../homotopy-equivalence.md) induces a [cohomology](../../../../cohomology-split.md)-ring isomorphism, **the [torus](../../../../torus.md) and this wedge are not [homotopy](../../../../homotopy-split.md) equivalent**.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../split.md)
5. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
