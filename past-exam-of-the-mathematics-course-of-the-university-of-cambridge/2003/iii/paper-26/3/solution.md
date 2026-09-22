<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use integral [singular homology](../../../../../singular-homology.md). The [singular chain group](../../../../../singular-chain-group.md) $C_n(B)$ is the [free abelian group](../../../../../free-abelian-group.md) on continuous maps $\Delta^n\to B$, and its [boundary operator](../../../../../boundary-operator.md) is

$$
\partial\sigma=\sum_{j=0}^n(-1)^j\sigma|_{[0,\ldots,\widehat j,\ldots,n]}.
$$

For $i<j$, deleting vertex $j$ and then vertex $i$ has sign $(-1)^{i+j}$, while deleting $i$ and then the shifted vertex $j-1$ has sign $(-1)^{i+j-1}$. Both yield the same codimension-two face. Pairing these terms proves $\partial^2=0$. The inclusion $A\subset B$ identifies $C_n(A)$ with the subgroup spanned by those simplices having image in $A$, so it is injective and preserved by $\partial$.

The [relative chain complex](../../../../../relative-chain-complex.md) is $C_n(B,A)=C_n(B)/C_n(A)$ with induced boundary $\partial\bar b=\overline{\partial b}$. Thus there is a degreewise [short exact sequence of chain complexes](../../../../../short-exact-sequence-of-chain-complexes.md)

$$
0\longrightarrow C_*(A)\xrightarrow{i}C_*(B)\xrightarrow{q}C_*(B,A)\longrightarrow0.
$$

Inclusion and quotient take [homological cycles](../../../../../chain-cycle.md) to [homological cycles](../../../../../chain-cycle.md) and boundaries to boundaries, hence define the [group homomorphisms](../../../../../group-homomorphism.md) $i_*$ and $q_*$ on [homology](../../../../../homology-split.md). We construct and prove exactness of the resulting sequence directly, rather than invoke an unproved algebraic lemma:

$$
\cdots\longrightarrow H_{n+1}(B,A)\xrightarrow{\delta}H_n(A)\xrightarrow{i_*}H_n(B)\xrightarrow{q_*}H_n(B,A)\xrightarrow{\delta}H_{n-1}(A)\longrightarrow\cdots
$$

ending in $H_0(A)\to H_0(B)\to H_0(B,A)\to0$.

For the [relative homology connecting homomorphism](../../../../../relative-homology-connecting-homomorphism.md), lift a [relative cycle](../../../../../relative-cycle.md) $\bar b\in C_n(B,A)$ to $b\in C_n(B)$. Since $\partial\bar b=0$, the chain $\partial b$ belongs to $C_{n-1}(A)$; it is a [homological cycle](../../../../../chain-cycle.md) because $\partial^2=0$. Define

$$
\delta[\bar b]=[\partial b]\in H_{n-1}(A).
$$

Changing the lift by $a\in C_n(A)$ changes the boundary by $\partial a$, hence does not change its [homology](../../../../../homology-split.md) class. More generally, if a different [relative cycle](../../../../../relative-cycle.md) represents the same [relative homology class](../../../../../relative-homology-class.md), lifts satisfy $b'-b=\partial c+a$ for some $c\in C_{n+1}(B)$ and $a\in C_n(A)$. Then $\partial b'-\partial b=\partial a$. This proves independence both of the lift and of the [homology](../../../../../homology-split.md) representative. Lifting a sum by the sum of lifts proves additivity, so $\delta$ is a well-defined [group homomorphism](../../../../../group-homomorphism.md).

At $H_n(A)$, an element in the image of $\delta$ is represented by $\partial b$ for some $b\in C_{n+1}(B)$, so its image in $H_n(B)$ is zero. Conversely, if a [homological cycle](../../../../../chain-cycle.md) in $A$ $a$ has $i_*[a]=0$, then $a=\partial b$ for a $B$-chain $b\in C_{n+1}(B)$. Its quotient $\bar b$ is a [relative cycle](../../../../../relative-cycle.md) and $\delta[\bar b]=[a]$. Thus

$$
\boxed{\operatorname{im}\bigl(\delta:H_{n+1}(B,A)\to H_n(A)\bigr)=\ker i_*.}
$$

For completeness, the other terms are exact by the same elementary chain argument. At $H_n(B)$, clearly $q_*i_*=0$. If a [homological cycle](../../../../../chain-cycle.md) in $B$ $b$ has zero relative class, then $\bar b=\partial\bar c$ for a quotient chain $\bar c$. Lifting $c$ gives $a=b-\partial c\in C_n(A)$, and $\partial a=0$. Hence $[b]=i_*[a]$, proving $\ker q_*=\operatorname{im}i_*$. At $H_n(B,A)$, absolute [homological cycles](../../../../../chain-cycle.md) have zero connecting image. Conversely, if $\delta[\bar b]=0$, then $\partial b=\partial a$ for some $a\in C_n(A)$; the chain $b-a$ is an absolute [homological cycle](../../../../../chain-cycle.md) and maps to $[\bar b]$. Therefore $\ker\delta=\operatorname{im}q_*$. In degree zero every quotient chain lifts to an absolute [homological cycle](../../../../../chain-cycle.md), because the differential to degree $-1$ is zero, so $q_*:H_0(B)\to H_0(B,A)$ is surjective. These proofs establish the whole [long exact sequence in relative homology](../../../../../long-exact-sequence-in-relative-homology.md) and all the algebraic facts used in its construction.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
