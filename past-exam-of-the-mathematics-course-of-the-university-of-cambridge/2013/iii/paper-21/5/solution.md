<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [idele group](../../../../../idele-group.md) is the multiplicative [restricted product](../../../../../restricted-product.md)

$$
J_K=\prod_v'K_v^\times
=\{(x_v):x_v\in K_v^\times,\ x_v\in\mathcal O_v^\times\text{ for all but finitely many finite }v\}.
$$

Its [restricted product topology](../../../../../restricted-product-topology.md) has basic open sets $\prod_{v\in S}U_v\times\prod_{v\notin S}\mathcal O_v^\times$, where $S$ is finite and contains every infinite place, and $U_v$ is open in $K_v^\times$. In particular, the restriction to almost all local [unit groups](../../../../../unit-group.md) is part of the topology, not merely the unrestricted product topology.

The diagonal map $K^\times\to J_K$ is injective and well-defined by finite support of the [principal ideal](../../../../../principal-ideal.md)'s [valuations](../../../../../valuation.md); its image consists of [principal ideles](../../../../../principal-idele.md). To prove [discreteness of principal ideles](../../../../../discreteness-of-principal-ideles.md), take the neighbourhood of $1$ which requires $x_v\in\mathcal O_v^\times$ at every finite place and $|x_v-1|<1/2$ in the ordinary real or complex modulus at every infinite place. A diagonal element in it is a global unit, so $x-1\in\mathcal O_K$. If $x\ne1$, the nonzero integer $N_{K/\mathbb Q}(x-1)$ has absolute value at least one, but the archimedean bounds make its absolute value less than $2^{-[K:\mathbb Q]}$. This contradiction proves **$K^\times$ is a discrete subgroup of $J_K$**.

For a [modulus of a number field](../../../../../modulus-of-a-number-field.md), write $\mathfrak m$ for its finite ideal part together with any selected real places. Let $I_{\mathfrak m}$ be the group of fractional ideals coprime to the finite part. Let $P_{\mathfrak m}$ consist of [principal ideals](../../../../../principal-ideal.md) $(a)$ with $a\equiv1\pmod{\mathfrak p_v^{m_v}}$ locally at each finite place in the modulus, and $a>0$ at each selected real place. The [ray class group](../../../../../ray-class-group.md) is

$$
\boxed{\operatorname{Cl}_{\mathfrak m}(K)=I_{\mathfrak m}/P_{\mathfrak m}.}
$$

Equivalently it is the quotient $J_K/(K^\times U_{\mathfrak m})$, with the corresponding principal-unit factors at finite places and positive multiplicative factors at selected real places. The question now assumes that no infinite places occur.

Put $R_{\mathfrak m}=\prod_{v\in S}\mathcal O_v^\times/(1+\pi_v^{m_v}\mathcal O_v)$. Global units map to $R_{\mathfrak m}$ by reduction. To map $R_{\mathfrak m}$ to the [ray class group](../../../../../ray-class-group.md), choose, by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md), an integral $a$ having the prescribed unit residues at all $v\in S$, and send the tuple to the ray class of $(a)$. A different choice changes the ratio by an element congruent to one at every such place, so the map is well-defined and multiplicative.

The forgetful map to the ordinary [ideal class group](../../../../../ideal-class-group.md) is surjective: [weak approximation for number fields](../../../../../weak-approximation-for-number-fields.md) multiplies an ideal by a [principal ideal](../../../../../principal-ideal.md) so that all its [valuations](../../../../../valuation.md) in $S$ vanish. Its kernel consists exactly of classes represented by [principal ideals](../../../../../principal-ideal.md) coprime to $S$, and their generators supply the local unit residues. Finally, a residue tuple maps to the identity ray class precisely when its chosen $a$ differs from a congruence-one generator by a global unit. Thus the [ray class exact sequence](../../../../../ray-class-exact-sequence.md) is

$$
\boxed{\mathcal O_K^\times\longrightarrow R_{\mathfrak m}\longrightarrow\operatorname{Cl}_{\mathfrak m}(K)\longrightarrow\operatorname{Cl}(K)\longrightarrow0.}
$$

The leftmost arrow need not be injective, explaining the absence of an initial zero.

For $K=\mathbb Q(\sqrt2)$, the [ring of integers of Q of square root two](../../../../../ring-of-integers-of-q-of-square-root-two.md) is $\mathbb Z[\sqrt2]$. Its absolute [field norm](../../../../../field-norm.md) is a Euclidean function. Indeed, for $a+b\sqrt2\in K$, choose nearest integers $m,n$; writing $u=a-m$, $w=b-n$, both bounded by $1/2$, gives $|u^2-2w^2|\leq1/2<1$. Applying this to a quotient proves [Euclidean division](../../../../../euclidean-division.md), hence the ring is a [principal ideal domain](../../../../../principal-ideal-domain.md) and $\operatorname{Cl}(K)=0$. This is [norm-Euclideanity of the integers adjoined square root two](../../../../../norm-euclideanity-of-the-integers-adjoined-square-root-two.md).

Write $\mathfrak p=(\sqrt2)$ and $\mathfrak q=(1+2\sqrt2)$. Their [ideal norms](../../../../../ideal-norm.md) are $2$ and $7$, respectively; $\mathfrak p^2=(2)$ and the [residue field](../../../../../residue-field.md) at $\mathfrak q$ is $\mathbb F_7$, with $\sqrt2\equiv3$ because $1+2\sqrt2\equiv0$. The finite local quotient product for the requested modulus is

$$
R_{\mathfrak m}\cong(\mathbb F_2[t]/(t^2))^\times\times\mathbb F_7^\times\cong C_2\times C_6.
$$

The first factor consists of $1$ and $1+t$.

The given [fundamental unit](../../../../../fundamental-unit-number-theory.md) $\epsilon=1+\sqrt2$ and $-1$ generate the global units. Their images are

$$
\epsilon\longmapsto(1+t,4),\qquad -1\longmapsto(1,6).
$$

The first image has order six; its cube is $(1+t,1)$ and its square is $(1,2)$, generating the first factor and the order-three subgroup of the second. The second image supplies the missing order-two element of $\mathbb F_7^\times$. Thus the global unit map is surjective onto all $12$ local unit residues. By the exact sequence, or the [unit-surjectivity criterion for a trivial finite ray class group](../../../../../unit-surjectivity-criterion-for-a-trivial-finite-ray-class-group.md),

$$
\boxed{\operatorname{Cl}_{2(v)+(v')}(\mathbb Q(\sqrt2))=0.}
$$

There is no positivity condition here: the modulus has no infinite part, so using the unit $-1$ is legitimate and essential in the surjectivity calculation.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
