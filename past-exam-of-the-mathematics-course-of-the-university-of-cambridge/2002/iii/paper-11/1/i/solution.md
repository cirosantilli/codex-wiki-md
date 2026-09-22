<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the pair-design convention: each pair of distinct points must lie in exactly one [Steiner block](../../../../../../block-of-a-steiner-system.md) of size $k$. With this convention the printed endpoint $k=1$ is false for every $v\geq2$, since a singleton contains no pair. Thus the intended assertion requires $k\geq2$. For $k=2$, take all pairs as [Steiner blocks](../../../../../../block-of-a-steiner-system.md) for any $v\geq2$. We now give a finite-field construction for every fixed $k\geq3$, without assuming the desired design-existence theorem.

Put $m=\binom{k}{2}$ and take an odd [prime](../../../../../../prime-number.md) power $q\equiv1\pmod{2m}$. By cyclicity of $\mathbb F_q^\times$, it has a [subgroup](../../../../../../subgroup.md) $H$ of index $m$; its order $(q-1)/m$ is even, so $-1\in H$. We will find a $k$-set $A=\{a_1,\ldots,a_k\}$ such that its $m$ unordered pair differences occupy the $m$ distinct [cyclotomic classes of a finite field](../../../../../../cyclotomic-class-of-a-finite-field.md) modulo $H$. The following argument supplies that set for every sufficiently large compatible $q$.

First establish the required two-class intersection estimate by elementary [character](../../../../../../character-of-a-representation.md) sums. Let $\chi$ be a [multiplicative character of a finite field](../../../../../../multiplicative-character-of-a-finite-field.md) of order $m$, with $\chi(\gamma)=\zeta_m$ for a generator $\gamma$. Extend every power $\chi^j$, including the trivial [character](../../../../../../character-of-a-representation.md), by zero at zero. For $C_i=\gamma^iH$,

$$
\mathbf1_{C_i}(x)=\frac1m\sum_{j=0}^{m-1}\zeta_m^{-ij}\chi^j(x).
$$

For a nontrivial additive [character](../../../../../../character-of-a-representation.md) $\psi$ of $\mathbb F_q$ and a nontrivial multiplicative [character](../../../../../../character-of-a-representation.md) $\eta$, its [Gauss sum of a finite-field character](../../../../../../gauss-sum-of-a-finite-field-character.md) satisfies

$$
|G(\eta)|^2
=\sum_{t\ne0}\eta(t)\sum_{y\ne0}\psi((t-1)y)
=(q-1)-\sum_{t\ne0,1}\eta(t)=q.
$$

Here the inner sum equals $q-1$ for $t=1$ and $-1$ otherwise, by additive-character [orthogonality](../../../../../../orthogonal-vectors.md); multiplicative-character [orthogonality](../../../../../../orthogonal-vectors.md) gives the last equality. Such a nontrivial additive [character](../../../../../../character-of-a-representation.md) exists by identifying the additive [group](../../../../../../group-split.md) with a [vector space](../../../../../../vector-space-split.md) over its [prime field](../../../../../../prime-field.md) and choosing a nonzero [linear functional](../../../../../../linear-functional.md) into that [prime field](../../../../../../prime-field.md).

If $\eta,\xi,\eta\xi$ are nontrivial, substituting $x=uz$, $y=(1-u)z$ in the product of their Gauss sums proves

$$
G(\eta)G(\xi)=J(\eta,\xi)G(\eta\xi),\qquad
J(\eta,\xi)=\sum_u\eta(u)\xi(1-u).
$$

The terms with $x+y=0$ sum to zero because $\eta\xi$ is nontrivial. Hence $|J|=\sqrt q$. If exactly one [character](../../../../../../character-of-a-representation.md) is trivial, subtracting the excluded zero and one terms gives absolute value one. If both are nontrivial but their product is trivial, the substitution $u/(1-u)$ gives $J(\eta,\eta^{-1})=-\eta(-1)$, again of absolute value one. If both are trivial, the sum is $q-2$. Expanding the two cyclotomic indicators and scaling a nonzero translate to one therefore gives, uniformly in $i,j$ and $t\ne0$,

$$
|C_i\cap(t+C_j)|=\frac{q}{m^2}+O_m(\sqrt q).
$$

All constants depend only on the fixed $m$.

To extend a prescribed difference pattern on $r$ coordinates, fix desired classes $D_1,\ldots,D_r$ for the new differences $x-a_i$ and set

$$
M(a)=\#\{x:x-a_i\in D_i\text{ for all }i\},\qquad a\in\mathbb F_q^r.
$$

Average over all $q^r$ tuples, allowing repeated coordinates just for this average. With $f=(q-1)/m$, counting choices for each $a_i$ independently gives

$$
\mathbb EM=q(f/q)^r=q/m^r+O_{m,r}(1).
$$

For the second moment, sum over the two potential extensions $x,y$. The $x=y$ terms contribute $qf^r/q^r$. For $x\ne y$, the choices of $a_i$ number $q/m^2+O_m(\sqrt q)$ each, by the preceding intersection estimate. Thus

$$
\mathbb EM^2=q^2/m^{2r}+O_{m,r}(q^{3/2}),\qquad
\operatorname{Var}M=O_{m,r}(q^{3/2}).
$$

The [Chebyshev inequality](../../../../../../chebyshev-inequality.md) shows that the proportion of tuples with $M(a)<q/(2m^r)$ is $O_{m,r}(q^{-1/2})$. Inductively, any fixed compatible difference pattern on $r$ distinct coordinates is realized by at least $c_rq^r$ tuples, with $c_r>0$ independent of sufficiently large $q$. The assertion starts with $r=1$. Almost all tuples are outside the exceptional set, so at least half the realizing tuples have at least $q/(2m^r)$ extensions. Each extension is distinct from the old coordinates because its differences belong to nonzero classes. This proves the assertion for $r+1$. This [cyclotomic pattern extension by a second-moment bound](../../../../../../cyclotomic-pattern-extension-by-a-second-moment-bound.md) avoids the false assumption that every partial choice can be extended.

Prescribe a different one of the $m$ [cosets](../../../../../../coset.md) to each pair $a_j-a_i$, $i<j$. Since $-1\in H$, changing an orientation does not change its [coset](../../../../../../coset.md), so the prescriptions are compatible. The preceding induction supplies $A$.

Choose $S\subset H$ containing one element from each pair $\{h,-h\}$. Form the [Steiner blocks](../../../../../../block-of-a-steiner-system.md)

$$
\mathcal B=\{sA+t:s\in S,\ t\in\mathbb F_q\}.
$$

For two distinct points $x,y$, their difference identifies exactly one unordered pair $\{a_i,a_j\}$ of $A$ having the same $H$-coset. Exactly one of $(x-y)/(a_i-a_j)$ and its negative lies in $S$. Choose the orientation $a,b$ of that pair making $s=(x-y)/(a-b)\in S$, and then set $t=x-sa$. This yields $x=sa+t$, $y=sb+t$. Both the oriented base pair and $(s,t)$ are unique, so precisely one [Steiner block](../../../../../../block-of-a-steiner-system.md) contains the pair. In particular different [Steiner block](../../../../../../block-of-a-steiner-system.md) parameters cannot produce repeated [Steiner blocks](../../../../../../block-of-a-steiner-system.md). Equivalently, the [Steiner blocks](../../../../../../block-of-a-steiner-system.md) $sA$ form a [difference family for a Steiner 2-design](../../../../../../difference-family-for-a-steiner-2-design.md), and translation gives the [cyclotomic construction of a Steiner 2-design](../../../../../../cyclotomic-construction-of-a-steiner-2-design.md).

There are infinitely many suitable [field](../../../../../../field.md) orders: choose one odd [prime](../../../../../../prime-number.md) $\ell$ not dividing $2m$, and take $q=\ell^{\varphi(2m)u}$ for [integers](../../../../../../integer.md) $u\geq1$. Euler's congruence gives $q\equiv1\pmod{2m}$, and these orders become arbitrarily large. Consequently

$$
\boxed{\text{For every }k\geq2,\text{ there are }2\text{-}(v,k,1)\text{ designs for infinitely many }v.}
$$

The qualification at $k=1$ is necessary for the standard pair-design definition.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
