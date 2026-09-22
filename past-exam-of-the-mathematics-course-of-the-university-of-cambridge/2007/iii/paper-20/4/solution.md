<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $V=\mathbb F_2^3$. Since $\mathbb F_2^\times=\{1\}$ and the [scalar](../../../../../scalar.md) centre is trivial,

$$
G=\mathrm{PSL}(3,2)=\mathrm{GL}(3,2),\qquad |G|=(8-1)(8-2)(8-4)=168.
$$

Choose $U_1$ to stabilize a nonzero [vector](../../../../../vector.md) and $U_2$ to stabilize a two-dimensional subspace. There are seven choices of either object, so both [subgroups](../../../../../subgroup.md) have index $7$ and order $24$.

Their coset [permutation characters](../../../../../permutation-character.md) agree. The number of nonzero [vectors](../../../../../vector.md) fixed by $g$ is $2^{\dim\ker(g-I)}-1$. A two-dimensional subspace is the kernel of a unique nonzero [covector](../../../../../covector.md), so its stabilizer action is the dual action $g^{-T}$. Its fixed-point count is

$$
2^{\dim\ker(g^{-T}-I)}-1=2^{\dim\ker(g-I)}-1,
$$

using equality of the [matrix ranks](../../../../../matrix-rank.md) of a [matrix](../../../../../matrix.md) and its transpose. For a [subgroup](../../../../../subgroup.md) $H$, counting the representatives of fixed cosets gives

$$
\chi_{G/H}(g)=\frac{|C_G(g)|}{|H|}\,|H\cap[g]_G|.
$$

Thus the equal characters and [subgroup](../../../../../subgroup.md) orders give equal intersection counts with every [conjugacy class](../../../../../conjugacy-class.md). This proves **$U_1,U_2$ are [Gassmann equivalent](../../../../../gassmann-equivalence.md)**.

They are not conjugate. For example, the stabilizer of $e_1$ contains every [matrix](../../../../../matrix.md) $\begin{pmatrix}1&b\\0&B\end{pmatrix}$ with $b\in\mathbb F_2^{1\times2}$ and $B\in\mathrm{GL}(2,2)$. An invariant plane containing $e_1$ would give an invariant line in $V/\langle e_1\rangle$, impossible for the full $\mathrm{GL}(2,2)$ action. An invariant plane not containing $e_1$ would be a complement to that line, but the arbitrary shears $b$ do not preserve any such complement. Hence a point stabilizer preserves no plane, whereas every conjugate of $U_2$ does. **The two [subgroups](../../../../../subgroup.md) are nonconjugate.**

We now use a [cone-torus construction of genus-four Sunada surfaces](../../../../../cone-torus-construction-of-genus-four-sunada-surfaces.md). Let $B$ be a hyperbolic torus with one cone point of angle $2\pi/7$. Its [orbifold fundamental group](../../../../../orbifold-fundamental-group.md) has presentation

$$
\Gamma=\langle a,d\mid[d,a]^7=1\rangle.
$$

Map $a,d$ to the supplied generators $A,D$ of $G$. Their commutator has exact order $7$, so this gives a surjection $\Gamma\to G$ with torsion-free kernel $K$: every finite-order element of $\Gamma$ is conjugate to a power of the cone generator, and no nonidentity such power lies in $K$. Thus $N=\mathbb H^2/K$ is a smooth closed [hyperbolic surface](../../../../../hyperbolic-surface.md) with a $G$-action. Its quotients by $U_1,U_2$ are smooth too, since order-$24$ [subgroups](../../../../../subgroup.md) contain no element of order $7$ and therefore meet no cone stabilizer.

The [orbifold Euler characteristic](../../../../../orbifold-euler-characteristic.md) of $B$ is $-(1-1/7)=-6/7$. Each quotient cover has degree $7$, so

$$
\chi(S_i)=7\chi_{\rm orb}(B)=-6=2-2g(S_i),\qquad
\boxed{g(S_1)=g(S_2)=4}.
$$

The [Sunada theorem](../../../../../sunada-theorem.md) proved in Question 3 makes $S_1,S_2$ isospectral for every choice of the base [hyperbolic metric](../../../../../hyperbolic-metric.md).

Here is an explicit supply of base metrics. A [hyperbolic trirectangle](../../../../../lambert-quadrilateral.md) has three right angles and a fourth angle $\alpha=\pi/14$. If its sides adjacent to the opposite right-angle vertex have lengths $r,s$, the trirectangle identity is $\sinh r\sinh s=\cos\alpha$. Thus $r>0$ varies freely, with $s=\operatorname{arsinh}(\cos\alpha/\sinh r)$. Reflecting four copies about their two perpendicular centre lines gives a quadrilateral with four angles $\pi/14$ and opposite sides of equal length. Identifying opposite sides produces a cone torus: all four corners give total angle $2\pi/7$. Its two centre-line [geodesics](../../../../../geodesic.md) intersect once and have lengths $2r,2s$. Cut along the shorter chosen [geodesic](../../../../../geodesic.md) $d$ and reglue with a small twist $\tau$; this retains the cone angle and allows an additional metric parameter. The remaining cut surface has two equal-length [geodesic](../../../../../geodesic.md) boundaries and the cone point.

We give a concrete [intersection test for nonisometric finite covers](../../../../../intersection-test-for-nonisometric-finite-covers.md), rather than relying on [subgroup](../../../../../subgroup.md) nonconjugacy alone. Choose $\ell(d)=\varepsilon$ sufficiently small. The trirectangle geometry gives an embedded collar of width $\log(1/\varepsilon)+O(1)$ about $d$. The shortest perpendicular joining the two boundary components after cutting has length $\delta=2\log(1/\varepsilon)+O(1)$. At zero twist it closes to $a$, the unique shortest [closed geodesic](../../../../../closed-geodesic.md) crossing $d$ once. Uniqueness follows from uniqueness of the shortest perpendicular; all other once-crossing classes have a positive length gap, since only finitely many [closed geodesics](../../../../../closed-geodesic.md) have bounded length. For sufficiently small twists, the same marked class $a$ remains the unique shortest once-crossing [geodesic](../../../../../geodesic.md). A [geodesic](../../../../../geodesic.md) crossing $d$ at least twice traverses the collar at least twice, so for small $\varepsilon$ its length is greater than $\ell(a)$.

[Geodesics](../../../../../geodesic.md) disjoint from $d$ remain entirely in the cut surface and have twist-independent lengths. In a bounded window around $\ell(a)$ they supply only finitely many possible length values, including lengths of iterates. Meanwhile $\ell(a)$ varies nontrivially with $\tau$ by the hyperbolic seam identity: its hyperbolic cosine has a positive multiple of $\cosh(\tau/2)$. Choose a small twist away from those finitely many coincidences. Then the only base [geodesic](../../../../../geodesic.md) of length $\ell(a)$ is $a$, up to [orientation](../../../../../orientation-of-a-simplex.md). By taking $\varepsilon$ smaller if necessary, the only base [geodesics](../../../../../geodesic.md) of length at most $2\varepsilon$ are powers of $d$: those crossing $d$ are long, and the nonperipheral [geodesics](../../../../../geodesic.md) of the limiting two-cusped cone pair of pants have lengths bounded away from zero.

In each cover, primitive lift components of a base [geodesic](../../../../../geodesic.md) are indexed by cycles of its [monodromy permutation](../../../../../monodromy-permutation.md), with length equal to the cycle size times its base length. The permutation of $A$ has a unique singleton $\{0\}$ in each action, so each $S_i$ has a uniquely length-identified primitive lift $\alpha_i$ of length $\ell(a)$. The permutation of $D$ has one two-cycle: it is $\{0,3\}$ for $U_1$ and $\{2,5\}$ for $U_2$. Hence each $S_i$ has a unique primitive lift $\beta_i$ of length $2\varepsilon$; the iterate of the singleton lift is not primitive. At the single base intersection of $a,d$, intersections of their lifted components are exactly their common sheet labels. Therefore

$$
\boxed{i(\alpha_1,\beta_1)=1,\qquad i(\alpha_2,\beta_2)=0}.
$$

An [isometry](../../../../../isometry.md) would have to preserve the uniquely identified primitive lengths and their [geometric intersection numbers](../../../../../geometric-intersection-number.md). This contradiction proves that $S_1$ and $S_2$ are not isometric, even allowing [orientation](../../../../../orientation-of-a-simplex.md) reversal.

Finally, let $\varepsilon$ range over a sufficiently small positive interval, choosing a permissible twist for each value. The singleton cycle of $D$ makes the [hyperbolic systole](../../../../../hyperbolic-systole.md) of each cover equal to $\varepsilon$. Distinct values therefore give distinct [isometry](../../../../../isometry.md) classes. We obtain **uncountably many pairs of nonisometric, isospectral [genus](../../../../../genus-of-a-surface.md)-four [Riemann surfaces](../../../../../riemann-surfaces.md)**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
