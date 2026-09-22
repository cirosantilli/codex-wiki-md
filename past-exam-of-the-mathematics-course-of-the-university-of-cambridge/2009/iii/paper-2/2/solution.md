<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Hall theorem for soluble groups](../../../../../hall-conjugacy-and-embedding-in-finite-soluble-groups.md) says that for every prime set $\pi$, a finite [soluble group](../../../../../solvable-group.md) has Hall $\pi$-subgroups; they are all conjugate, and every $\pi$-subgroup is contained in one. A Hall $\pi$-subgroup has only primes in $\pi$ in its order and no primes in $\pi$ in its index.

For a proof outline, induct on the [group](../../../../../group-split.md) order and choose a [minimal normal subgroup](../../../../../minimal-normal-subgroup.md) $N$. In a finite [soluble group](../../../../../solvable-group.md) this is elementary abelian of some characteristic $p$: its derived [subgroup](../../../../../subgroup.md) is characteristic and solvability forces it to be trivial; primary components and the [subgroup](../../../../../subgroup.md) of elements of order dividing $p$ are then characteristic, so minimality gives an [elementary abelian p-group](../../../../../elementary-abelian-group.md). Choose a Hall $\pi$-subgroup of $G/N$ and let $U$ be its preimage. If $p\in\pi$, $U$ is itself a Hall $\pi$-subgroup. If $p\notin\pi$, $U/N$ has order prime to $p$ and [coprime splitting over an elementary abelian normal subgroup](../../../../../coprime-splitting-over-an-elementary-abelian-normal-subgroup.md) supplies a complement to $N$ in $U$, of the required Hall order.

Here the complement fact has a short averaging proof. Choose a section of $U/N=H$ and write its multiplication defect as $f(h,k)\in N$, in additive notation. Associativity gives

$$
f(h,k)+f(hk,t)=h f(k,t)+f(h,kt).
$$

Since $|H|$ is invertible on $N$, averaging over $t$ expresses the defect as $f(h,k)=b(h)+h b(k)-b(hk)$; adjusting the section by $-b$ gives a homomorphic section. Two such complements differ by $d(hk)=d(h)+h d(k)$. Averaging this identity gives $d(h)=b-hb$, so they are conjugate by $b\in N$. Inductive conjugacy in the quotient followed by this complement conjugacy proves Hall conjugacy. To embed an arbitrary $\pi$-subgroup $Q$, first put its quotient inside the chosen quotient [Hall subgroup](../../../../../hall-subgroup.md). In the coprime case $Q$ and the corresponding [subgroup](../../../../../subgroup.md) of a complement are both complements to $N$ inside $NQ$, hence are $N$-conjugate. In the other case $Q\le U$ directly. This proves [Hall conjugacy and embedding in finite soluble groups](../../../../../hall-conjugacy-and-embedding-in-finite-soluble-groups.md) as well as existence.

Now prove the assertion about [maximal subgroups](../../../../../maximal-subgroup.md) by induction on $|G|$. Suppose a nontrivial [normal subgroup](../../../../../normal-subgroup.md) $K$ is contained in $A$. If $K\not\le B$, maximality gives $KB=G$, and since $K\le A$ this gives $AB=G$. If $K\le B$, both $A/K$ and $B/K$ are maximal in $G/K$; induction yields either their product equal to $G/K$ or their conjugacy, lifting respectively to $AB=G$ or to conjugacy of $A,B$. The same applies with their roles reversed.

It remains to suppose that no nontrivial [normal subgroup](../../../../../normal-subgroup.md) of $G$ lies in either maximum. Let $K$ be minimal normal, an [elementary abelian p-group](../../../../../elementary-abelian-group.md). Since $K$ lies in neither maximum, $KA=KB=G$. The intersection $K\cap A$ is normalized by $A$ and by the [abelian group](../../../../../abelian-group.md) $K$, hence by $G$; it is therefore trivial. Likewise $K\cap B=1$. Thus both $A$ and $B$ complement $K$. Their action on $K$ is irreducible, since an [invariant subspace](../../../../../invariant-subspace.md) would be a proper nontrivial [normal subgroup](../../../../../normal-subgroup.md) of $G$. It is also faithful: $C_A(K)$ is normalized by $A$ and centralized by $K$, so is a [normal subgroup](../../../../../normal-subgroup.md) of $G$ contained in $A$ and must be trivial.

If $G/K=1$, these assumptions force $A=B=1$ and $G$ to have prime order. Otherwise choose $L>K$ normal in $G$ with $L/K$ minimal normal in $G/K$. It is an elementary abelian r-group. Under $A\cong G/K$, its copy $R=A\cap L$ is a nontrivial [normal subgroup](../../../../../normal-subgroup.md) of $A$. The prime $r$ differs from $p$: a [p-group](../../../../../p-group.md) acting on the characteristic-p [vector space](../../../../../vector-space-split.md) $K$ has nonzero fixed points, by counting its orbits on $K$ modulo $p$. Its fixed subspace would be $A$-invariant, hence all of $K$ by irreducibility, contrary to faithfulness of $R$.

Therefore $A\cap L$ and $B\cap L$ are Sylow r-subgroups of $L=K(A\cap L)=K(B\cap L)$. They are conjugate in $L$. Conjugate $B$ so that these intersections coincide as $R$. Since $R\lhd A$, $N_G(R)\ge A$. It cannot equal $G$, since $R$ would then be a nontrivial [normal subgroup](../../../../../normal-subgroup.md) contained in $A$. Maximality gives $N_G(R)=A$, and the same argument gives $N_G(R)=B$. The conjugated maxima are equal. Hence

$$
\boxed{G=AB\quad\text{or}\quad A\text{ and }B\text{ are conjugate in }G.}
$$

This is the factorization-or-conjugacy property of [maximal subgroups of a finite soluble group](../../../../../maximal-subgroups-of-a-finite-soluble-group.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
