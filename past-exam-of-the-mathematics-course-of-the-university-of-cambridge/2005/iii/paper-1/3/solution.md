<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose a minimal nontrivial [normal subgroup](../../../../../normal-subgroup.md) $L$ of $K$ itself. Every conjugate $L^g$ for $g\in G$ is also a [minimal normal subgroup](../../../../../minimal-normal-subgroup.md) of $K$, since $K$ is normal in $G$. Distinct such subgroups intersect trivially: their intersection is normal in $K$ and minimality forces either equality or trivial intersection. Moreover $[L_i,L_j]\subseteq L_i\cap L_j=1$, so distinct ones commute.

Choose a maximal family of these conjugates whose product $M=L_1\times\cdots\times L_r$ is direct. For any further conjugate $L^g$, its intersection with $M$ is normal in $K$ and is either all of $L^g$ or trivial. In the latter case it commutes with all the existing factors and could be adjoined to the [direct product of groups](../../../../../direct-product-of-groups.md), contrary to maximality. Thus every conjugate is contained in $M$. The product of all conjugates is consequently $M$, which is nontrivial and normal in $G$. Minimality of $K$ as a $G$-normal subgroup gives $M=K$.

Any [normal subgroup](../../../../../normal-subgroup.md) of a factor $L_i$ is normal in $K$: the other direct factors commute with it, and $L_i$ normalizes it. Minimality of $L_i$ as a $K$-normal subgroup makes it simple. All factors are isomorphic because they are conjugate to $L$. This proves the [direct-product structure of a finite minimal normal subgroup](../../../../../direct-product-structure-of-a-finite-minimal-normal-subgroup.md):

$$
\boxed{K\cong S^r\quad\text{for a finite simple group }S.}
$$

An abelian [simple group](../../../../../simple-group.md) is cyclic of prime order, so the abelian case is elementary abelian. Now let $H$ be a maximal proper subgroup of a nonabelian [simple group](../../../../../simple-group.md) $X$. It is nontrivial, since $X$ has nontrivial proper [cyclic subgroups](../../../../../cyclic-subgroup.md). Choose a [minimal normal subgroup](../../../../../minimal-normal-subgroup.md) $K$ of $H$. Then $H\le N_X(K)$. This [normalizer](../../../../../normalizer.md) cannot be $X$, since that would make $1<K\le H<X$ normal in $X$. Maximality gives

$$
\boxed{H=N_X(K),\qquad K\cong S^r.}
$$

For each of the two groups in this question, the allowed absence of proper nonabelian simple subgroups makes the factors of such a $K$ cyclic of prime order. Hence it suffices to examine [normalizers](../../../../../normalizer.md) of nontrivial elementary abelian subgroups.

In $A_5$, the possible primes are two, three and five. The [Sylow subgroups](../../../../../sylow-subgroup.md) for the last two primes are cyclic of orders three and five. Every involution is a double [transposition](../../../../../transposition-permutation.md); for $(12)(34)$ the [centralizer](../../../../../centralizer.md) in $A_5$ is

$$
\{1,(12)(34),(13)(24),(14)(23)\},
$$

the [Klein four-group](../../../../../klein-four-group.md) fixing point five. Thus an elementary abelian $2$-subgroup is cyclic of order two or a [Klein four-group](../../../../../klein-four-group.md). The [normalizer](../../../../../normalizer.md) of a cyclic order-two subgroup equals its [centralizer](../../../../../centralizer.md) and has order four, so is contained in a point [stabilizer](../../../../../stabilizer-subgroup.md) of order twelve. A [Klein four-group](../../../../../klein-four-group.md)'s common fixed point is intrinsic, and the full point [stabilizer](../../../../../stabilizer-subgroup.md) $A_4$ normalizes it; its [normalizer](../../../../../normalizer.md) is therefore exactly that [stabilizer](../../../../../stabilizer-subgroup.md).

An order-three subgroup has support a triple. Its [normalizer](../../../../../normalizer.md) preserves the triple and the remaining pair, and is $(S_3\times S_2)\cap A_5$, of order six. An order-five subgroup acts regularly on all five points. Label the points by $\mathbb F_5$, with the subgroup acting by translations. Its [normalizer](../../../../../normalizer.md) in $S_5$ is the twenty affine maps $x\mapsto ax+b$. The translations are even, whereas multiplication by a generator of $\mathbb F_5^{\times}$ is a four-cycle and is odd. Exactly half these maps are even, so the [normalizer](../../../../../normalizer.md) in $A_5$ has order ten.

The only candidates for [maximal subgroups](../../../../../maximal-subgroup.md) are thus the [normalizers](../../../../../normalizer.md) of orders twelve, ten and six. They are all maximal: none can lie in a larger candidate, except potentially an order-six subgroup in an order-twelve $A_4$. But an index-two subgroup of $A_4$ would contain every order-three element; there are eight such elements, plus the identity, already more than six. Hence that containment is impossible. Point [stabilizers](../../../../../stabilizer-subgroup.md) are conjugate; order-three and order-five subgroup [normalizers](../../../../../normalizer.md) each form one class by the [Sylow theorems](../../../../../sylow-theorems.md). Therefore the [maximal subgroups of A5](../../../../../maximal-subgroups-of-a5.md) form precisely

$$
\boxed{\text{three conjugacy classes, of orders }12,10,6.}
$$

Their numbers are five, six and ten respectively, since these proper [maximal subgroups](../../../../../maximal-subgroup.md) are self-normalizing in the [simple group](../../../../../simple-group.md).

For $X=GL_3(2)$, choosing independent columns gives $|X|=(8-1)(8-2)(8-4)=168$. If $t$ is an involution, write $t=I+N$. [Field characteristic](../../../../../characteristic-of-a-field.md) two gives $N^2=0$, and $\operatorname{im}N\subseteq\ker N$ in dimension three forces its nonzero rank to be one. Thus $t=I+vf$, with nonzero vector $v$, nonzero [linear functional](../../../../../linear-functional.md) $f$ and $f(v)=0$. This [transvection](../../../../../transvection.md) fixes the plane $\ker f$ and has image line $\langle v\rangle$. Every flag consisting of an incident line and plane occurs, giving $7\cdot3=21$ involutions, all conjugate. Its [centralizer](../../../../../centralizer.md), and hence the [normalizer](../../../../../normalizer.md) of its [cyclic subgroup](../../../../../cyclic-subgroup.md), is the flag [stabilizer](../../../../../stabilizer-subgroup.md) of order $168/21=8$. It lies in both the line and plane [stabilizers](../../../../../stabilizer-subgroup.md) of order $24$, so cannot be maximal.

For the [elementary abelian subgroups in GL3 over F2](../../../../../elementary-abelian-subgroups-in-gl3-over-f2.md), consider commuting [transvections](../../../../../transvection.md) $I+vf$, $I+wh$. Their rank-one parts satisfy

$$
v f(w)h=w h(v)f.
$$

If $v,w$ are independent, equality forces both sides zero; thus $f,h$ vanish on $\langle v,w\rangle$ and are the same nonzero functional. If $v=w$, they have a common image line. Consequently the two types of order-four elementary abelian subgroup are

$$
K_L=\{I+vf:f(v)=0\},\qquad
K_W=\{I+wf:w\in W=\ker f\}.
$$

No extra [transvection](../../../../../transvection.md) can commute with all elements of $K_L$: if its image were different, its functional would have to equal each of the two independent functionals occurring in $K_L$. Dually, the same holds for $K_W$. Thus these exhaust the elementary abelian $2$-subgroups of rank at least two. The [normalizer](../../../../../normalizer.md) of $K_L$ is the line [stabilizer](../../../../../stabilizer-subgroup.md) and the [normalizer](../../../../../normalizer.md) of $K_W$ is the plane [stabilizer](../../../../../stabilizer-subgroup.md), each of order $168/7=24$. They give different [conjugacy classes](../../../../../conjugacy-class.md) because their common fixed spaces have dimensions one and two. All line [stabilizers](../../../../../stabilizer-subgroup.md) are conjugate, as are all plane [stabilizers](../../../../../stabilizer-subgroup.md).

For an order-three element, its [minimal polynomial](../../../../../minimal-polynomial.md) is $(X-1)(X^2+X+1)$: it has a fixed line and an invariant complementary irreducible plane. Its [normalizer](../../../../../normalizer.md) preserves both and is the full $GL_2(2)$ on that plane, of order six, since the order-three subgroup is normal in $GL_2(2)$. This [normalizer](../../../../../normalizer.md) lies in the corresponding line and plane [stabilizers](../../../../../stabilizer-subgroup.md), so is not maximal.

An order-seven element is irreducible. Over the [finite field](../../../../../finite-field.md) $\mathbb F_2$ one has $X^7-1=(X-1)(X^3+X+1)(X^3+X^2+1)$, and both cubic factors are irreducible because neither has a root in $\mathbb F_2$. Its [minimal polynomial](../../../../../minimal-polynomial.md) divides this square-free product and cannot be just $X-1$, since the element is not the identity. It therefore contains a cubic factor; the three-dimensional space forces that irreducible cubic to be the whole [minimal polynomial](../../../../../minimal-polynomial.md). Identify the space with $\mathbb F_8$ and the element with multiplication by a generator $\alpha$ of $\mathbb F_8^{\times}$. Its [centralizer](../../../../../centralizer.md) consists of the seven nonzero multiplication maps. A [normalizer](../../../../../normalizer.md) induces an $\mathbb F_2$-automorphism of this field, so it sends $\alpha$ to $\alpha$, $\alpha^2$ or $\alpha^4$. All three possibilities occur via the field [automorphisms](../../../../../automorphism.md) $x\mapsto x^{2^j}$. Therefore the [normalizer](../../../../../normalizer.md) of the [Singer cycle](../../../../../singer-cycle.md) has order $7\cdot3=21$, and all such [normalizers](../../../../../normalizer.md) are conjugate by the [Sylow theorems](../../../../../sylow-theorems.md).

The maximal-normalizer reduction leaves exactly the two order-twenty-four [stabilizer](../../../../../stabilizer-subgroup.md) types and the order-twenty-one type. Each is maximal because it cannot be contained in any larger remaining candidate; equal-order subgroups cannot properly contain one another and $21$ does not divide $24$. Thus

$$
\boxed{GL_3(2)\text{ has exactly three maximal-subgroup classes, of orders }24,24,21.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
