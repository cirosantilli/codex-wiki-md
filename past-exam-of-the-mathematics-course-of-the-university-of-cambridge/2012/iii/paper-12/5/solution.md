<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $m=\operatorname{ord}(A)$, $n=\operatorname{ord}(B)$ and $r=\operatorname{ord}(AB)$. Cut the [Riemann sphere](../../../../../riemann-sphere.md) along arcs joining three marked points, say $0,1,\infty$, so the complement is [simply connected](../../../../../simply-connected-space.md). Take copies labeled by the elements of $T$ and glue the slit banks with monodromies given by left multiplication by $A,B,(AB)^{-1}$. The product relation ensures consistency. The surface is connected because $A,B$ generate $T$. At a puncture with monodromy order $m$, fill each cycle using the local complex coordinate $z=w^m$; use the analogous charts at the other two punctures. This constructs the [three-branch-point regular surface cover](../../../../../three-branch-point-regular-surface-cover.md) $N\to\mathbb P^1$.

Right multiplication by inverses defines a left action of $T$, commutes with the monodromy gluing and extends holomorphically over the filled points. Average a compatible metric over this finite group to obtain a metric for which $T$ acts by [Riemannian isometries](../../../../../riemannian-isometry.md). When the genus is at least two, the unique compatible curvature-minus-one metric from the [uniformization theorem](../../../../../uniformization-theorem.md) is an invariant choice. Away from the three marked fibers the action is free. The nontrivial [stabilizer subgroups](../../../../../stabilizer-subgroup.md) are the conjugates of $\langle A\rangle$, $\langle B\rangle$ and $\langle AB\rangle$, of orders $m,n,r$, omitting order-one groups.

There are $|T|/m$, $|T|/n$, $|T|/r$ points over the corresponding branch points. The [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) gives

$$
\boxed{\chi(N)=|T|\left(\frac1m+\frac1n+\frac1r-1\right).}
$$

This construction also covers the spherical and toroidal cases. If one monodromy has order one it is simply an unbranched marked fiber, with no nontrivial stabilizer.

For the supplied coset actions, faithfulness gives $m=n=3$. Compose permutations with the rightmost factor acting first. The two products $AB$ have cycle decompositions

$$
\begin{aligned}
\rho_1(AB)&=(1\ 5\ 12\ 6\ 3\ 9)(2\ 8\ 7\ 4\ 11\ 10),\\
\rho_2(AB)&=(1\ 5\ 9\ 6\ 3\ 12)(2\ 8\ 7\ 4\ 11\ 10).
\end{aligned}
$$

Thus $r=6$. The index is twelve and each [subgroup](../../../../../subgroup.md) has order eight, so $|T|=96$. Consequently

$$
\boxed{\chi(N)=96(1/3+1/3+1/6-1)=-16,\qquad g(N)=9.}
$$

All cycles of $A,B,AB$ on each coset set have the full orders $3,3,6$. No nontrivial power of any of these branch monodromies fixes a coset. The fixed-coset criterion means that each $U_i$ has trivial intersection with every conjugate of each cyclic branch stabilizer. Since these are all stabilizers on $N$, both $U_i$ act freely. Their quotient surfaces are therefore smooth closed surfaces, not cone-point orbifolds. [Sunada theorem](../../../../../sunada-theorem.md) supplies isospectrality, and the unbranched [Euler characteristic](../../../../../euler-characteristic.md) formula gives

$$
\boxed{\chi(U_i\backslash N)=-16/8=-2,\qquad g(U_i\backslash N)=2.}
$$

Choose the hyperbolic metric for these surfaces and their common genus-nine cover.

In this natural construction the two genus-two surfaces are **isometric**, by an orientation-reversing map. Define the sheet permutation

$$
P=(1\ 2)(4\ 6)(7\ 10)(8\ 12)(9\ 11).
$$

Direct composition verifies

$$
\boxed{P\rho_1(A)P^{-1}=\rho_2(A)^{-1},\qquad
P\rho_1(B)P^{-1}=\rho_2(B)^{-1}.}
$$

Complex conjugation of the base sphere fixes its three real branch points and reverses the two chosen generating loops, so their monodromies become the inverses. These identities supply a lift, after relabeling sheets by $P$, to an anticonformal map between the two branched covers. It extends across the branch points by the local power charts. An anticonformal map between closed hyperbolic [Riemann surfaces](../../../../../riemann-surfaces.md) is a [Riemannian isometry](../../../../../riemannian-isometry.md), by uniqueness of the compatible hyperbolic metric.

Equivalently, take the [hyperbolic triangle group](../../../../../hyperbolic-triangle-group.md) of signature $(3,3,6)$. Reflection in the side joining the two order-three vertices conjugates its two vertex rotations to their inverses. The displayed sheet permutation identifies the reflected [subgroup](../../../../../subgroup.md) for the first covering with the [subgroup](../../../../../subgroup.md) for the second, up to an irrelevant change of base sheet. This is the [orientation-reversing equivalence of branched-cover monodromy](../../../../../orientation-reversing-equivalence-of-branched-cover-monodromy.md). The exhibited isometry is anticonformal, so the conclusion is about [Riemannian isometry](../../../../../riemannian-isometry.md), without asserting that this map is holomorphic. Merely knowing the [subgroups](../../../../../subgroup.md) were almost conjugate would not have settled isometry; the explicit inverse-monodromy symmetry does. Nor does the data force this symmetry for every arbitrarily chosen invariant deformation of the cover's metric: it is present for the constructed hyperbolic metric.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
