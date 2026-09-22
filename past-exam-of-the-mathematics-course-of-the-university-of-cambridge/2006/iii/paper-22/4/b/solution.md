<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $k=e(E)=c_2(E)[X]=1$, where the underlying oriented real rank-four bundle has its complex orientation. The charge-one [Uhlenbeck-Donaldson compactness for charge-one ASD connections](../../../../../../uhlenbeck-donaldson-compactness-for-charge-one-asd-connections.md) assertion is that any sequence of [ASD connections](../../../../../../anti-self-dual-connection.md) $A_n$ has a subsequence with one of these alternatives: modulo [bundle gauge transformations](../../../../../../unitary-bundle-gauge-transformation.md), it converges smoothly on all of $X$ to an [ASD connection](../../../../../../anti-self-dual-connection.md) of charge one; or it converges smoothly on compact subsets of $X\setminus\{x\}$ to a connection that extends smoothly on a charge-zero bundle and is flat, with

$$
\boxed{|F_{A_n}|^2\,d\mathrm{vol}_g\ \rightharpoonup\ 8\pi^2\delta_x.}
$$

Bundle identifications are made on the complement of the bubble point in the second alternative. In general the flat limit can have nontrivial holonomy; trivial charge does not imply trivial connection on an arbitrary base. The closure of the charge-one moduli space in the ideal-instanton topology adds only a subset of $M_0\times X$, and is compact. Here $M_0$ denotes flat gauge classes on charge-zero bundles.

The local analytic inputs are the following, stated so that the compactness conclusion is not itself assumed. A [Uhlenbeck small-energy Coulomb gauge](../../../../../../uhlenbeck-small-energy-coulomb-gauge.md) on a four-ball exists whenever $\int_B|F_A|^2$ is below a universal local threshold; it obeys $d^*a=0$, the usual normal boundary condition, and $\|a\|_{W^{1,2}}\leq C\|F_A\|_2$ after rescaling. For [ASD connections](../../../../../../anti-self-dual-connection.md), the local small-energy regularity estimates bound every [vector-bundle curvature](../../../../../../curvature-form.md) derivative on a smaller ball:

$$
\sup_{B_{r/2}}|\nabla_A^mF_A|
\leq C_m r^{-2-m}\|F_A\|_{L^2(B_r)}.
$$

Together with [elliptic regularity](../../../../../../elliptic-regularity.md) in the Coulomb gauge, these give bounds on all derivatives of local [connection matrices](../../../../../../connection-one-form.md) on smaller balls. Smooth fixed metrics permit these estimates on sufficiently small coordinate balls. Finally, the [Uhlenbeck removable singularity theorem for ASD connections](../../../../../../uhlenbeck-removable-singularity-theorem-for-asd-connections.md) states that a smooth finite-energy [ASD connection](../../../../../../anti-self-dual-connection.md) on a punctured four-ball extends smoothly after a gauge change and bundle extension. Rellich compactness and elliptic bootstrapping are used in passing from bounded local representatives to smooth subsequential limits. These are local estimates and an extension theorem, not the global bubbling theorem being proved.

For the proof, put the inner product $\langle U,V\rangle=-\operatorname{Tr}(UV)$ on the anti-Hermitian Lie algebra. Since $*F_A=-F_A$,

$$
\operatorname{Tr}(F_A\wedge F_A)
=-\operatorname{Tr}(F_A\wedge*F_A)=|F_A|^2\,d\mathrm{vol}_g.
$$

Thus every $A_n$ has energy $8\pi^2$. Pass to a weakly convergent subsequence of the nonnegative curvature-energy measures. Let $S$ be the points at which the limit measure has an atom at least the small-energy threshold. There are finitely many, because the total mass is fixed.

At every point outside $S$, a sufficiently small ball has limit mass less than the threshold; choose its boundary to have zero limit mass. The corresponding energies for all large $n$ are then below the threshold. The local Coulomb gauges and the stated estimates yield smooth subsequential convergence on smaller balls. A countable cover and diagonal extraction give these limits everywhere outside $S$. On overlaps, the transition gauges satisfy the first-order equation relating the two [connection matrices](../../../../../../connection-one-form.md). Their derivatives are bounded by the already controlled matrices, and the compactness of $SU(2)$ controls their zeroth-order values. Extracting limits of these transitions patches the local limits into a smooth bundle and [ASD connection](../../../../../../anti-self-dual-connection.md) $A_\infty$ on $X\setminus S$. On a fixed compact subset, close transition cocycles identify the original and limiting bundles by smooth near-identity isomorphisms; one can construct these by embedding the bundles into one trivial Hermitian bundle and using the polar decomposition of the nearby orthogonal projections. This yields actual bundle identifications for the convergent connections, not merely separate local limits.

The limiting [vector-bundle curvature](../../../../../../curvature-form.md) has finite energy by lower semicontinuity. Apply the removable-singularity input at each point of $S$. We obtain a smooth extended bundle $E_\infty$ and [ASD connection](../../../../../../anti-self-dual-connection.md) on all of $X$. Strong convergence away from $S$ shows that the remaining measure is a nonnegative sum of atoms:

$$
|F_{A_n}|^2d\mathrm{vol}_g\ \rightharpoonup\
|F_{A_\infty}|^2d\mathrm{vol}_g+\sum_{p\in S}\beta_p\delta_p,
\qquad \beta_p>0.
$$

Discard any artificial zero-defect points if they occur in a preliminary choice of exceptional set.

Here is the topological argument that makes the defects integral, rather than merely small positive real numbers. Around one point $p$, choose a ball $B$ whose boundary contains no exceptional point. Both the original and the extended limiting bundles are trivial over $B$, but their gauges identifying the boundary can differ by a map $S^3\to SU(2)$. The [Second Chern number](../../../../../../second-chern-number.md) of the clutching bundle obtained by gluing two copies of $B$ is an integer. Using the [Chern-Simons three-form](../../../../../../chern-simons-3-form.md) on the boundary gives

$$
\frac1{8\pi^2}\left(\int_B\operatorname{Tr}(F_{A_n}\wedge F_{A_n})
-\int_B\operatorname{Tr}(F_{A_\infty}\wedge F_{A_\infty})\right)
=N_n+o(1),\qquad N_n\in\mathbb Z.
$$

The $o(1)$ term is the difference of the boundary Chern-Simons integrals in the convergent gauges, hence tends to zero by smooth boundary convergence. The integer is the clutching contribution. The left side tends to $\beta_p/(8\pi^2)$, so the closedness of $\mathbb Z$ gives $\beta_p=8\pi^2m_p$ for an integer $m_p\geq1$.

Taking total masses now gives

$$
\boxed{1=k(E_\infty)+\sum_{p\in S}m_p},\qquad
k(E_\infty)=\frac{\|F_{A_\infty}\|_2^2}{8\pi^2}\in\mathbb Z_{\geq0}.
$$

There are only two possibilities. If the sum is zero, there is no concentration; the same local gauges cover all of $X$, giving smooth gauge convergence on the original bundle. If the sum is nonzero, it consists of one integer one, and $k(E_\infty)=0$. The limiting [vector-bundle curvature](../../../../../../curvature-form.md) therefore vanishes, and all energy is the single atom $8\pi^2\delta_x$. This proves the alternatives.

Finally, flat gauge classes on a compact base form a compact space: choose finitely many generators of its [fundamental group](../../../../../../fundamental-group.md), identify flat classes with the closed representation subset of a finite product of $SU(2)$ subject to its relations, and quotient by the compact conjugation action. All flat $SU(2)$ bundles here have zero second Chern class and the corresponding charge-zero topological type. Thus the ideal stratum $M_0\times X$ is compact. Combining its subsequential compactness with the two alternatives proves compactness of the closure in the ideal-instanton topology. No gluing theorem asserting that every formal ideal point is realized is needed for this compactness statement.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
