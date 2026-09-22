<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We regard $N$ as positive and invertible in $k$; $N=1$ gives the trivial group and the same arguments apply. Put $A=\operatorname{Pic}^0(C)$, an [abelian variety](../../../../../abelian-variety-split.md) of dimension $g$.

First compute the [prime-to-characteristic torsion of an abelian variety](../../../../../prime-to-characteristic-torsion-of-an-abelian-variety.md). The differential of $[N]:A\to A$ at the origin is $N\operatorname{id}$, and translation gives the same assertion everywhere. Consequently $[N]$ is an [étale morphism](../../../../../etale-morphism.md), its fibres have dimension zero, and properness makes it finite. Its image is closed of dimension $g$, hence all of $A$. Choose an [ample line bundle](../../../../../ample-line-bundle.md) $L_0$ on $A$ and put $L=L_0\otimes[-1]^*L_0$, which is symmetric and ample. The [Theorem of the Cube](../../../../../theorem-of-the-cube.md) gives the recurrence

$$
[n+1]^*L\otimes[n-1]^*L\cong([n]^*L)^{\otimes2}\otimes L^{\otimes2}.
$$

After fixing a trivialization at the origin, induction from $n=0,1$ gives $[n]^*L\cong L^{\otimes n^2}$. Comparing top [intersection products](../../../../../intersection-product-of-cartier-divisors.md) under the finite map $[N]$ gives

$$
\deg[N]\,(c_1(L)^g)=(c_1([N]^*L)^g)=N^{2g}(c_1(L)^g).
$$

The intersection number is positive because $L$ is ample, so $\deg[N]=N^{2g}$. Since $[N]$ is étale and $k$ is [algebraically closed field](../../../../../algebraically-closed-field.md), its kernel has precisely $N^{2g}$ points.

For a prime power $\ell^r\mid N$, write the [finite abelian group](../../../../../finite-abelian-group.md) $A[\ell^r]$ as a product of cyclic groups of orders $\ell^{a_j}$, with $1\le a_j\le r$. Its subgroup killed by $\ell$ is $A[\ell]$, so the number of factors is $2g$. Its total order is $\ell^{2gr}$, so $\sum a_j=2gr$ forces every $a_j=r$. Combining the prime-power factors by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) proves

$$
\boxed{A[N]\cong(\mathbb Z/N\mathbb Z)^{2g}.}
$$

The same reasoning works for the [dual abelian variety](../../../../../dual-abelian-variety.md) $\widehat A$, also of dimension $g$.

To define the [Weil pairing for an abelian variety](../../../../../weil-pairing-for-an-abelian-variety.md) on two copies of $A[N]$, we first justify the required theta identification with $\widehat A$. Identify $X=\operatorname{Pic}^{g-1}(C)$ with an $A$-torsor and use ordinary translation $T_q(x)=x+q$. The [Theorem of the square](../../../../../theorem-of-the-square.md), a consequence of the [Theorem of the Cube](../../../../../theorem-of-the-cube.md), makes

$$
\lambda(q)=T_q^*\mathcal O_X(\Theta)\otimes\mathcal O_X(\Theta)^{-1}
$$

a [group homomorphism](../../../../../group-homomorphism.md) $A\to\widehat A$. Fix the negative [Abel map of an algebraic curve](../../../../../abel-map-of-an-algebraic-curve.md) $j:C\to A$, $P\mapsto[P_0-P]$, and let $\rho:\widehat A\to\operatorname{Pic}^0(C)=A$ be pullback by $j$. Pullback by a translate of $j$ gives the same map: algebraically trivial [line bundles](../../../../../line-bundle.md) on an [abelian variety](../../../../../abelian-variety-split.md) are translation-invariant as Picard classes, by the [Theorem of the square](../../../../../theorem-of-the-square.md).

For any $q\in A$, choose a degree-$g$ class $D$ such that both $D$ and $D+q$ have one-dimensional section spaces. This is possible because the nonspecial degree-$g$ classes form a nonempty open subset of the irreducible [Picard scheme of a curve](../../../../../picard-scheme-of-a-curve.md), and its translate has a nonempty intersection with it. Since $T_q\phi_D=\phi_{D+q}$, the [restriction of the theta divisor to an Abel curve](../../../../../restriction-of-the-theta-divisor-to-an-abel-curve.md) proved above gives

$$
\phi_D^*\lambda(q)\cong\mathcal O_C(D+q)\otimes\mathcal O_C(D)^{-1}\cong q.
$$

Each $\phi_D$ differs from $j$ by a translation. Thus $\rho\lambda=\operatorname{id}_A$. This equality on closed points is equality of morphisms, since $A$ is reduced and the target is separated. In particular $\lambda$ is a closed immersion, being a section of the separated morphism $\rho$. Its image has dimension $g=\dim\widehat A$, so it is all of the reduced irreducible [abelian variety](../../../../../abelian-variety-split.md) $\widehat A$. Therefore $\lambda$ is an isomorphism of [schemes](../../../../../scheme.md). This proves the needed [theta autoduality of a Jacobian](../../../../../theta-autoduality-of-a-jacobian.md), including possible infinitesimal issues in positive characteristic.

Here is a definition of the [Weil pairing for an abelian variety](../../../../../weil-pairing-for-an-abelian-variety.md) that also proves nondegeneracy. For $M\in\widehat A[N]$, the [Theorem of the Cube](../../../../../theorem-of-the-cube.md) gives $[N]^*M\cong M^{\otimes N}\cong\mathcal O_A$. Choose a trivialization of $[N]^*M$. The finite étale cover $[N]:A\to A$ has deck group $G=A[N]$. Its natural descent action on $[N]^*M$ becomes multiplication by scalars under this trivialization: these scalars are constant because every invertible regular function on the proper connected [abelian variety](../../../../../abelian-variety-split.md) $A$ is constant. They form a character

$$
\chi_M:G\longrightarrow k^\times,
$$

whose values lie in $\mu_N$, since $NP=0$ for every $P\in G$. Rescaling the trivialization changes none of these scalars. Translation gives multiplicativity in $P$, and [tensor product](../../../../../tensor-product.md) gives $\chi_{M\otimes M'}=\chi_M\chi_{M'}$. Define

$$
\boxed{e_N(P,Q)=\chi_{\lambda(Q)}(P)\in\mu_N.}
$$

This fixes a convention for the [Weil pairing for an abelian variety](../../../../../weil-pairing-for-an-abelian-variety.md); reversing the convention for the descent action inverts all values and changes no nondegeneracy assertion.

If $\chi_M=1$, the trivialization is equivariant for the deck group. Descent then makes $M$ the trivial [line bundle](../../../../../line-bundle.md) on the target. Thus

$$
\widehat A[N]\longrightarrow\operatorname{Hom}(A[N],\mu_N),\qquad M\longmapsto\chi_M
$$

is injective. The source and target both have $N^{2g}$ elements, since $k$ contains all $N$ distinct roots of unity and $A[N]\cong(\mathbb Z/N)^{2g}$. Hence it is an isomorphism. Characters of this group separate its points, so the [Weil pairing for an abelian variety](../../../../../weil-pairing-for-an-abelian-variety.md) is nondegenerate in both variables. Composing with the isomorphism $\lambda$ proves **the pairing on $A[N]$ is perfect**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
