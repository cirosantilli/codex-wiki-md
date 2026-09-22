<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Hall subgroup](../../../../../hall-subgroup.md) for a set of primes $\pi$ is a [subgroup](../../../../../subgroup.md) $H\leq G$ such that every prime divisor of $|H|$ belongs to $\pi$, while no prime divisor of $[G:H]$ belongs to $\pi$. Equivalently $|H|=|G|_\pi$, the product of the full prime powers in $|G|$ belonging to $\pi$.

The [Hall conjugacy and embedding in finite soluble groups](../../../../../hall-conjugacy-and-embedding-in-finite-soluble-groups.md) theorem says that, for every $\pi$, a finite [soluble group](../../../../../solvable-group.md) has a Hall $\pi$-subgroup, any two such [subgroups](../../../../../subgroup.md) are conjugate, and every $\pi$-subgroup is contained in one. We prove all three assertions together by induction, including the needed complement argument rather than assuming it.

First establish [coprime splitting over an elementary abelian normal subgroup](../../../../../coprime-splitting-over-an-elementary-abelian-normal-subgroup.md). Suppose $V\trianglelefteq E$ is an elementary [Abelian](../../../../../abelian-group.md) $r$-group and $D=E/V$ has order $m$ prime to $r$. Write $V$ additively. [Conjugation](../../../../../conjugation.md) defines a well-defined action of $D$ on $V$ because $V$ is [Abelian](../../../../../abelian-group.md). Choose a section $s:D\to E$, with $s(1)=1$, and let its [extension cocycle](../../../../../extension-cocycle.md) be defined by $s(x)s(y)=f(x,y)s(xy)$. Associativity gives

$$
f(x,y)+f(xy,z)=x f(y,z)+f(x,yz).
$$

Sum over $z\in D$. With $S(x)=\sum_z f(x,z)$ this becomes

$$
mf(x,y)+S(xy)=xS(y)+S(x).
$$

Multiplication by $m$ is invertible on $V$, so setting $b(x)=m^{-1}S(x)$ gives $f(x,y)=b(x)+xb(y)-b(xy)$. The new section $s'(x)=(-b(x))s(x)$ has zero cocycle and is a homomorphism. Its image is a complement $K$ to $V$, proving $E=V\rtimes K$.

Every other complement has the form $\{h(x)s'(x):x\in D\}$, with $h(xy)=h(x)+xh(y)$. Summing this identity over $y$ and putting $T=\sum_y h(y)$ gives $mh(x)=T-xT$. Hence $h(x)=v-xv$, where $v=m^{-1}T$, and the other complement is $vKv^{-1}$. The same argument applies on any [subgroup](../../../../../subgroup.md) $D_0\leq D$: a [subgroup](../../../../../subgroup.md) intersecting $V$ trivially is a graph of such a one-cocycle over its image $D_0$, so [conjugation](../../../../../conjugation.md) by an element of $V$ carries it into $K$. This proves the complement-conjugacy and embedding assertions needed below.

Now let $G\ne1$ be finite soluble, and choose a [minimal normal subgroup](../../../../../minimal-normal-subgroup.md) $V$. It is elementary [Abelian](../../../../../abelian-group.md) of some prime characteristic $r$, by the minimal-normal argument in the series discussion. Induction gives Hall [subgroups](../../../../../subgroup.md) and the embedding and conjugacy assertions in $G/V$. Let $\overline H$ be a Hall $\pi$-subgroup there and $M$ its full preimage.

If $r\in\pi$, then $M$ itself is a Hall $\pi$-subgroup of $G$. Every Hall $\pi$-subgroup $H$ contains $V$, since $HV$ is a $\pi$-subgroup and $H$ already has the largest possible $\pi$-order. Thus $H$ is the full preimage of its image in $G/V$, and quotient conjugacy lifts to conjugacy in $G$. Given any $\pi$-subgroup $U$, induction puts its quotient image into some $\overline H$, whose preimage $M$ contains $U$.

If $r\notin\pi$, then $M/V=\overline H$ has order prime to $r$. The complement construction produces $K\leq M$ of order $|\overline H|=|G|_\pi$, hence a Hall [subgroup](../../../../../subgroup.md) of $G$. Any Hall [subgroup](../../../../../subgroup.md) has trivial intersection with $V$ and a Hall image in $G/V$. Conjugating two Hall [subgroups](../../../../../subgroup.md) first aligns these images, after which both are complements to $V$ in the same $M$; the complement-conjugacy argument then conjugates them by an element of $V$. For an arbitrary $\pi$-subgroup $U$, quotient induction puts its image into some $\overline H$. Then $U\subseteq M$ and $U\cap V=1$, so the embedding argument conjugates $U$ into the chosen complement $K$. Equivalently $U$ lies in a conjugate of $K$. This completes the induction and all three parts of the [Hall theorem for soluble groups](../../../../../hall-conjugacy-and-embedding-in-finite-soluble-groups.md).

For the specific [general linear group over a finite field](../../../../../general-linear-group-over-a-finite-field.md), counting ordered bases gives

$$
|GL_3(2)|=(8-1)(8-2)(8-4)=168.
$$

There are seven lines and seven planes in $\mathbb F_2^3$. The [group](../../../../../group-split.md) is transitive on each family, so line and plane stabilizers both have order $24$ and index seven. To show that these exhaust the index-seven [subgroups](../../../../../subgroup.md), let $H$ have order $24$. It contains a Sylow $2$-subgroup of order eight, which can be conjugated to

$$
U=\left\{\begin{pmatrix}1&a&b\\0&1&d\\0&0&1\end{pmatrix}:a,b,d\in\mathbb F_2\right\}.
$$

The [group orbits](../../../../../orbit-of-a-group-action.md) of $U$ on the seven nonzero [vectors](../../../../../vector.md) are

$$
\{e_1\},\quad\{e_2,e_1+e_2\},\quad
\{e_3,e_1+e_3,e_2+e_3,e_1+e_2+e_3\},
$$

of sizes $1,2,4$. An $H$-orbit is a union of these. The [group](../../../../../group-split.md) $H$ cannot be transitive on seven points, since seven does not divide $24$. Therefore it has an orbit of size at most three. A size-one orbit fixes $e_1$. A size-two orbit must be $\{e_2,e_1+e_2\}$, whose [vector](../../../../../vector.md) sum $e_1$ is consequently fixed. A size-three orbit must be the union of the first two $U$-orbits, the nonzero part of the plane $\langle e_1,e_2\rangle$, so that plane is invariant. In every case $H$ lies in a line or plane stabilizer, and equality follows from their equal orders.

The two stabilizer families are not conjugate. A line stabilizer fixes its nonzero [vector](../../../../../vector.md) and is transitive on the other six nonzero [vectors](../../../../../vector.md): extend that fixed [vector](../../../../../vector.md) and either chosen other [vector](../../../../../vector.md) to a basis, and map one such basis to the other. Thus it has no invariant three-element subset of nonzero [vectors](../../../../../vector.md) and fixes no plane. In contrast a plane stabilizer fixes its defining plane. [Conjugation](../../../../../conjugation.md) sends line stabilizers to line stabilizers, so cannot send one to a plane stabilizer. We obtain

$$
\boxed{\text{Exactly two conjugacy classes of index-seven subgroups: line stabilizers and plane stabilizers.}}
$$

They are [Hall subgroups](../../../../../hall-subgroup.md) for $\pi=\{2,3\}$ but are not conjugate. This explicitly shows why the solubility hypothesis of the [Hall theorem for soluble groups](../../../../../hall-conjugacy-and-embedding-in-finite-soluble-groups.md) matters.

Finally, an index-three [subgroup](../../../../../subgroup.md) would give a nontrivial transitive [coset](../../../../../coset.md) homomorphism $GL_3(2)\to S_3$. Its kernel is normal; the permitted simplicity of $GL_3(2)$ forces that kernel to be trivial, because the action is nontrivial. But an injective map from a [group](../../../../../group-split.md) of order $168$ into one of order six is impossible. Hence **$GL_3(2)$ has no [subgroup](../../../../../subgroup.md) of index three**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
