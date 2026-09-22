<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $C=\check\sigma=\sigma^\vee$, $S=C\cap M$, and $U_\sigma=X_{\check\sigma}=\operatorname{Spec}k[S]$. The [semigroup algebra](../../../../../semigroup-algebra.md) has basis $\chi^m=x^m$, $m\in S$, with $\chi^m\chi^{m'}=\chi^{m+m'}$. The vertex assumption means that $\sigma$ is strongly convex, so its [dual cone](../../../../../dual-cone.md) $C$ has full dimension. By the [Gordan lemma](../../../../../gordan-lemma.md), $S$ is finitely generated: choose integral [toric cone](../../../../../cone-in-toric-geometry.md) generators and subtract integer parts of their nonnegative coefficients; the remainder lies in a bounded parallelepiped with only finitely many lattice points. This argument also applies when $C$ has [lineality space](../../../../../lineality-space.md), by including generators in both directions there.

Choose an integral interior point $u\in C$. For every $m\in M$, both $tu$ and $tu+m$ belong to $S$ for all sufficiently large integers $t$. Thus $S-S=M$. Inverting all [monomial](../../../../../monomial.md) generators of $k[S]$ gives the [group algebra](../../../../../group-algebra.md) $k[M]$, which becomes $k[z_1^{\pm1},\ldots,z_n^{\pm1}]$ after a basis of $M$ is chosen. This proves the [dense torus of an affine toric variety](../../../../../dense-torus-of-an-affine-toric-variety.md) assertion:

$$
\boxed{X_M=\operatorname{Spec}k[M]\cong(k^*)^n\text{ is a dense open subset of }U_\sigma.}
$$

Density follows because the [localization of a ring](../../../../../localization-of-a-ring.md) is of a domain. The algebra map $\chi^m\mapsto\chi^m\otimes\chi^m$ from $k[S]$ to $k[M]\otimes k[S]$ defines the extended [algebraic torus](../../../../../algebraic-torus.md) action; on $X_M$ it is ordinary multiplication.

For a [face of a polyhedral cone](../../../../../face-of-a-polyhedral-cone.md) $\nu\preceq C$, set $I_\nu=(\chi^m:m\in S\setminus\nu)$. The [convex face](../../../../../face-of-a-convex-set.md) property ensures that this is an ideal, and quotienting leaves $k[\nu\cap M]$. Hence $X_\nu=\operatorname{Spec}k[\nu\cap M]$ is a closed subvariety of $U_\sigma$. Its open [algebraic torus](../../../../../algebraic-torus.md) consists of points where precisely the [monomials](../../../../../monomial.md) with exponent in $\nu$ are nonzero.

To see that these [algebraic tori](../../../../../algebraic-torus.md) exhaust the points, let $p$ be a point of $U_\sigma$ and put $S_p=\{m\in S:\chi^m(p)\ne0\}$. Multiplicativity gives $m+m'\in S_p$ if and only if both $m,m'\in S_p$. Thus $S_p$ is a [semigroup face](../../../../../face-of-an-additive-monoid.md). It is $S\cap\nu$ for a unique polyhedral [convex face](../../../../../face-of-a-convex-set.md) $\nu$: among a finite generating set of $S$, take the [toric cone](../../../../../cone-in-toric-geometry.md) spanned by generators nonzero at $p$. A relation expressing a sum with a generator outside this [toric cone](../../../../../cone-in-toric-geometry.md) as a combination of generators inside would, after clearing rational denominators, contradict the displayed multiplicativity property. Therefore the [toric cone](../../../../../cone-in-toric-geometry.md) is a [convex face](../../../../../face-of-a-convex-set.md). Conversely, if $m\in S$ lies in that [convex face](../../../../../face-of-a-convex-set.md), a positive multiple of $m$ is an integral sum of those generators, so $\chi^m(p)$ is nonzero as well. This also proves uniqueness.

The point $p$ lies in $X_M$ exactly when its [convex face](../../../../../face-of-a-convex-set.md) is all of $C$. Therefore

$$
\boxed{U_\sigma\setminus X_M=\bigcup_{\nu\prec C}X_\nu.}
$$

One can equivalently write this as the disjoint union of the open [algebraic tori](../../../../../algebraic-torus.md) of the proper [convex faces](../../../../../face-of-a-convex-set.md). For $\mu\in S$, the same description shows that $\chi^\mu(p)=0$ exactly when $\mu$ is not in the [convex face](../../../../../face-of-a-convex-set.md) supporting $p$. On every $X_\nu$ with $\mu\notin\nu$ the [monomial](../../../../../monomial.md) vanishes identically. Consequently the [monomial zero locus in an affine toric variety](../../../../../monomial-zero-locus-in-an-affine-toric-variety.md) is

$$
\boxed{V(\chi^\mu)_{\mathrm{red}}=\bigcup_{\substack{\nu\preceq C\\\mu\notin\nu}}X_\nu.}
$$

This is an equality of reduced subvarieties, or of their underlying closed sets. The principal subscheme itself may have multiplicity, as $x^2=0$ already shows on $\mathbb A^1$.

The [face duality for polyhedral cones](../../../../../face-duality-for-polyhedral-cones.md) is the order-reversing pair of maps

$$
\boxed{\tau\preceq\sigma\ \longmapsto\ C\cap\tau^\perp,\qquad \nu\preceq C\ \longmapsto\ \sigma\cap\nu^\perp.}
$$

Their values are [convex faces](../../../../../face-of-a-convex-set.md) because the relevant pairings are nonnegative and a sum pairs to zero only if each summand does. More explicitly, finitely many nonnegative exposing functionals can be summed to expose the indicated intersection. For a [convex face](../../../../../face-of-a-convex-set.md) $\tau$, choose $m_0\in C$ exposing it: $\tau=\sigma\cap m_0^\perp$. Then $m_0\in C\cap\tau^\perp$, so $\sigma\cap(C\cap\tau^\perp)^\perp\subseteq\tau$, while the reverse inclusion is immediate. Apply the same argument to a [convex face](../../../../../face-of-a-convex-set.md) $\nu$ of $C$, using $C^\vee=\sigma$, to prove the other composite is the identity. Inclusion reversal follows directly from annihilators. This proves the bijection, not just the existence of the maps.

For $\tau\preceq\sigma$, write $\nu=C\cap\tau^\perp$ and $L=M\cap\tau^\perp$. An exposing functional $m_0$ for $\tau$ is strictly positive on every [toric ray](../../../../../ray-of-a-fan.md) outside $\tau$. Small perturbations of $m_0$ within $\tau^\perp$ preserve those finitely many strict inequalities, so $\nu$ has nonempty [relative interior](../../../../../relative-interior.md) in $\tau^\perp$ and spans it. Therefore $\nu\cap M$ generates $L$, by the interior-point argument used above within that subspace. Thus the open [algebraic torus](../../../../../algebraic-torus.md) of $X_\nu$ is $\operatorname{Spec}k[L]=X_{\tau^\perp}$. Here $X_{\tau^\perp}$ uses the lattice in the whole annihilator, rather than the [toric cone](../../../../../cone-in-toric-geometry.md) semigroup. The sublattice $L$ is a [saturated sublattice](../../../../../saturated-sublattice.md) of $M$ and consequently a direct summand; restriction $\operatorname{Hom}(M,k^*)\to\operatorname{Hom}(L,k^*)$ is surjective. The extended [algebraic torus](../../../../../algebraic-torus.md) action is multiplication on this open [algebraic torus](../../../../../algebraic-torus.md) and hence transitive. All other [monomials](../../../../../monomial.md) vanish there. It follows that

$$
\boxed{O(\tau)=X_{\tau^\perp},\qquad F_\tau=\overline{O(\tau)}=X_{C\cap\tau^\perp}.}
$$

This is the [torus orbit-cone correspondence](../../../../../orbit-cone-correspondence.md) and its [orbit closure in a toric variety](../../../../../orbit-closure-in-a-toric-variety.md) description. Under [convex face](../../../../../face-of-a-convex-set.md) duality, $F_\gamma=\bigcup_{\eta\succeq\gamma}O(\eta)$.

Finally, choose integral $m_\tau\in C$ exposing $\tau$. Localizing $k[C\cap M]$ at $\chi^{m_\tau}$ gives $k[\tau^\vee\cap M]$: for $m\in\tau^\vee\cap M$, adding a sufficiently large multiple of $m_\tau$ makes it nonnegative on every [toric ray](../../../../../ray-of-a-fan.md) of $\sigma$ outside $\tau$, while preserving nonnegativity on $\tau$. Hence $X_{\check\tau}=U_\tau=D(\chi^{m_\tau})$ is the usual affine open chart inside $U_\sigma$. An orbit $O(\gamma)$ belongs to it exactly when $\gamma\preceq\tau$. The requested [complement of an affine toric face chart](../../../../../complement-of-an-affine-toric-face-chart.md) is therefore

$$
\boxed{X_{\check\sigma}\setminus X_{\check\tau}=\bigcup_{\substack{\gamma\preceq\sigma\\\gamma\npreceq\tau}}F_\gamma.}
$$

All sets on the right are closed, and if $\gamma$ is not contained in $\tau$, neither is any [convex face](../../../../../face-of-a-convex-set.md) containing $\gamma$. This justifies replacing the excluded orbits by their whole closures.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
