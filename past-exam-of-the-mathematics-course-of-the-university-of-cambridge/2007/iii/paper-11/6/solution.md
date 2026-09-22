<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [hyperbolic Riemann surface in potential theory](../../../../../hyperbolic-riemann-surface-in-potential-theory.md) is a noncompact [Riemann surface](../../../../../riemann-surfaces.md) admitting a positive [Green function on a Riemann surface](../../../../../green-function-on-a-riemann-surface.md). With pole $p$, this is a positive function harmonic off $p$, having local form $-\log|\zeta|$ plus a harmonic function in a coordinate $\zeta(p)=0$, and obtained as the minimal such positive function by exhaustion. This is a noncircular definition for the present proof. For a simply connected surface it is equivalent to disk conformal type; for arbitrary surfaces potential-theoretic hyperbolicity and disk universal-cover type should be distinguished.

The [unit disk](../../../../../unit-disk.md) is an example. At pole zero its function is $G(z,0)=-\log|z|$: it is positive in the punctured disk, harmonic there, has the correct logarithmic singularity, and tends to zero at the boundary. If another positive function has the same singularity and is harmonic elsewhere, subtract $G$ and apply the [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md) on disks of radius $r<1$; the boundary lower bound is $\log r$. Letting $r\uparrow1$ shows that the other function dominates $G$. Thus $G$ is indeed the positive [Green function on a Riemann surface](../../../../../green-function-on-a-riemann-surface.md). At a general pole it is

$$
\boxed{G(z,p)=\log\left|\frac{1-\overline pz}{z-p}\right|.}
$$

Here is a [Green-function exhaustion proof of disk uniformization](../../../../../green-function-exhaustion-proof-of-disk-uniformization.md). The main analytic idea is to build conformal maps on bordered disks from their Green functions and pass to an extremal limit. The positive global Green function prevents that limit from becoming constant.

First exhaust the noncompact simply connected surface $R$ by relatively compact domains $R_n$ containing $p$, each with a smooth Jordan boundary. This topological step does not use conformal uniformization: take regular neighborhoods of finitely many coordinate disks covering successive compact sets and fill bounded complementary components. Simple connectedness and the [Jordan curve theorem](../../../../../jordan-curve-theorem.md) make the filled neighborhoods topological disks; enlarge them to be nested.

Each $R_n$ has a zero-boundary [Green function on a Riemann surface](../../../../../green-function-on-a-riemann-surface.md) $G_n(\cdot,p)$. One analytic construction, independent of conformal uniformization, is as follows. Equip the compact bordered domain with a smooth [conformal metric](../../../../../conformal-metric.md). Multiply $-\log|\zeta|$ by a smooth [cutoff function](../../../../../cutoff-function.md) equal to one near $p$ and zero near the boundary; call the result $s$. Distributionally

$$
-\Delta s=2\pi\delta_p+k,
$$

where $k$ is smooth and supported away from $p$. Solve $\Delta v=k$ with zero boundary data. This auxiliary [Dirichlet problem](../../../../../dirichlet-problem.md) can be obtained by minimizing $\frac12\int|\nabla v|^2+\int kv$ over functions with zero boundary trace: the [Poincaré inequality](../../../../../poincare-inequality.md) gives [coercivity](../../../../../coercive-function.md), minimization in a [Hilbert space](../../../../../hilbert-space-split.md) gives a [weak solution](../../../../../weak-solution.md), and interior and smooth-boundary [elliptic regularity](../../../../../elliptic-regularity.md) give a smooth solution. Then $G_n=s+v$ is harmonic away from $p$, has the logarithmic pole, and vanishes at the boundary. It is positive by the [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md), applied after removing a sufficiently small circle around its positive pole. This construction uses ordinary linear elliptic existence, not the desired uniformization theorem. Equivalently, the same bordered-domain Green functions can be constructed by the [Perron method for the Dirichlet problem](../../../../../perron-method.md) using local logarithmic barriers.

On $R_n\setminus\{p\}$ choose local [harmonic conjugates](../../../../../harmonic-conjugate.md) $G_n^*$. Their period around the pole is $-2\pi$, and every closed loop is homologous to an integer multiple of that loop. Therefore

$$
f_n=\exp(-G_n-iG_n^*)
$$

is a single-valued [holomorphic function](../../../../../holomorphic-function.md). It extends across $p$ with one simple zero and has no others. Since $G_n>0$, $|f_n|<1$; since $G_n=0$ on the boundary, $|f_n|\to1$ there. Thus $f_n:R_n\to\mathbb D$ is proper. For any $a\in\mathbb D$, choose a smooth interior contour sufficiently close to the boundary that $|f_n|>|a|$ everywhere on it. The contour surrounds $p$ and all possible preimages of $a$, because $|f_n|>|a|$ throughout a thin boundary collar. By [Rouché's theorem](../../../../../rouche-s-theorem.md), $f_n-a$ has the same number of zeros inside as $f_n$, namely one. Hence $f_n$ is onto and one-to-one, with nonzero derivative: it is a [biholomorphism](../../../../../biholomorphism.md) from $R_n$ to the disk.

Write near $p$

$$
G_n=-\log|\zeta|+c_n+o(1).
$$

Multiply $f_n$ by a unit constant so that, in the fixed coordinate, $f_n'(p)=e^{-c_n}>0$. Domain monotonicity gives $G_n\leq G_{n+1}$: their difference is harmonic even at $p$ and nonnegative on $\partial R_n$. The global positive [Green function on a Riemann surface](../../../../../green-function-on-a-riemann-surface.md) $G_R$ similarly majorizes every $G_n$. Comparing the regular parts shows that $c_n$ increases and is bounded above by the finite regular part of $G_R$ at $p$. Consequently

$$
f_n'(p)\longrightarrow d>0.
$$

On each fixed compact subdomain, the $f_n$ are eventually bounded [holomorphic functions](../../../../../holomorphic-function.md). [Montel theorem](../../../../../montel-s-theorem.md) and a diagonal subsequence therefore give a [locally uniform convergence](../../../../../locally-uniform-convergence.md) limit $F:R\to\mathbb D$ with $F(p)=0$ and $F'(p)=d>0$. The [maximum modulus principle](../../../../../maximum-modulus-principle.md) keeps its values strictly inside the disk. It is injective: for fixed $q$, the functions $f_n-f_n(q)$ have no zeros away from $q$; [Hurwitz's theorem](../../../../../hurwitz-s-theorem.md) implies that their nonconstant limit has no other zeros. This is the [locally uniform limit of univalent functions](../../../../../locally-uniform-limit-of-univalent-functions.md) argument.

There is also an extremality property. For any [holomorphic function](../../../../../holomorphic-function.md) $g:R\to\mathbb D$ with $g(p)=0$, the function $g\circ f_n^{-1}$ is a disk self-map fixing zero. The [Schwarz lemma](../../../../../schwarz-lemma.md) gives $|g'(p)|\leq f_n'(p)$. Passing to the limit yields $|g'(p)|\leq d=F'(p)$.

Finally suppose $F$ omits $a\in\mathbb D$. Necessarily $a\ne0$. Apply the disk [Möbius transformation](../../../../../mobius-transformation.md) $\phi_a(w)=(w-a)/(1-\overline aw)$. The nowhere-zero function $\phi_a\circ F$ has a global [holomorphic logarithm](../../../../../holomorphic-logarithm.md) because $R$ is [simply connected](../../../../../simply-connected-space.md), hence a [holomorphic square root](../../../../../holomorphic-square-root.md) $h$. It maps into the disk and $|h(p)|=\sqrt{|a|}$. Normalize it by setting $g=\phi_{h(p)}\circ h$, so $g(p)=0$. Direct differentiation gives

$$
|g'(p)|=\frac{1-|a|^2}{2\sqrt{|a|}(1-|a|)}|F'(p)|=\frac{1+|a|}{2\sqrt{|a|}}d>d.
$$

The strict inequality follows from $(1-\sqrt{|a|})^2>0$. This contradicts extremality. Therefore $F$ omits no point, and we conclude

$$
\boxed{R\text{ is conformally equivalent to }\mathbb D.}
$$

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
