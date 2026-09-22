<h1 id="9g/solution">Solution</h1>

↑ **Parent:** [9G](../9g.md)

For subgroups $H,P\leq G$, define $x\sim y$ when $y\in HxP$. The identity elements show reflexivity, inverses show symmetry, and multiplication shows transitivity. Thus the [double cosets](../../../../../double-coset.md) $HxP$ partition $G$.

Let $H$ act by left multiplication on the set of left [cosets](../../../../../coset.md) $G/P$. The orbit of $xP$ consists of the cosets contained in $HxP$, so its size is $|HxP|/|P|$. Its stabilizer is

$$
\begin{aligned}
\operatorname{Stab}_H(xP)
&=\{h\in H:hxP=xP\}\\
&=H\cap xPx^{-1}.
\end{aligned}
$$

The [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) therefore gives

$$
\boxed{\frac{|HxP|}{|P|}
=\frac{|H|}{|H\cap xPx^{-1}|}}.
$$

Suppose $P$ is a [Sylow subgroup](../../../../../sylow-subgroup.md) of $G$, with $|P|=p^a$, and write the largest power of $p$ dividing $|H|$ as $p^b$. If every $H\cap xPx^{-1}$ had order at most $p^{b-1}$, the displayed formula would make every double-coset size divisible by $p^{a+1}$. Their sum $|G|$ would then also be divisible by $p^{a+1}$, contradicting the choice of $P$. Hence some $H\cap xPx^{-1}$ has order $p^b$ and is a Sylow $p$-subgroup of $H$. This is the [Sylow subgroup of a subgroup from double cosets](../../../../../sylow-subgroup-of-a-subgroup-from-double-cosets.md) argument.

To count the [general linear group over a finite field](../../../../../general-linear-group-over-a-finite-field.md) $GL_n(\mathbb F_p)$, choose its columns successively. There are $p^n-1$ choices for the first, $p^n-p$ for the second, and $p^n-p^k$ for column $k+1$. Consequently

$$
\boxed{|GL_n(\mathbb F_p)|
=\prod_{k=0}^{n-1}(p^n-p^k)
=p^{n(n-1)/2}\prod_{j=1}^n(p^j-1)}.
$$

None of the factors $p^j-1$ is divisible by $p$, so the [upper unitriangular group](../../../../../upper-unitriangular-group.md) is a Sylow $p$-subgroup: it has one arbitrary field entry in each of the $n(n-1)/2$ positions above the diagonal and hence order $p^{n(n-1)/2}$. The [permutation matrices](../../../../../permutation-matrix.md) form a subgroup isomorphic to the [symmetric group](../../../../../symmetric-group.md) $S_n$.

By [Cayley theorem](../../../../../cayley-s-theorem.md), every finite group $G$ embeds in $S_{|G|}$, and permutation matrices embed this symmetric group in $GL_{|G|}(\mathbb F_p)$. The latter has the explicit Sylow $p$-subgroup just described, so the result proved in the first part, applied to the embedded copy of $G$, proves that every finite group has a Sylow $p$-subgroup.

The counting part of the [Sylow theorems](../../../../../sylow-theorems.md) says that if $p^a$ is the largest power of $p$ dividing $|G|$, then the number $n_p$ of Sylow $p$-subgroups satisfies

$$
\boxed{n_p\equiv1\pmod p,\qquad n_p\mid |G|/p^a}.
$$

Finally, let $|G|=pq$ with prime numbers $p>q$. The Sylow counts give

$$
n_p\mid q,\quad n_p\equiv1\pmod p,
$$

so $n_p=1$ and the Sylow $p$-subgroup is a [normal subgroup](../../../../../normal-subgroup.md). Also $n_q\mid p$ and $n_q\equiv1\pmod q$. If $n_q=1$, both Sylow subgroups are normal; their elements commute, so $G$ is their [direct product](../../../../../direct-product-of-groups.md) and is [abelian](../../../../../abelian-group.md). In the nonabelian case one must therefore have $n_q=p$, whence

$$
\boxed{p\equiv1\pmod q},
$$

or equivalently $q\mid p-1$, as recorded by [nonabelian group of order pq](../../../../../nonabelian-group-of-order-pq.md).

## ↑ Ancestors (10)

1. [9G](../9g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
