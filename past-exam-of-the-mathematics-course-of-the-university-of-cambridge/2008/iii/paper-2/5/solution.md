<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The algebraic characterization is the [Boone-Higman theorem](../../../../../boone-higman-theorem.md):

$$
\boxed{G\text{ has soluble word problem}\quad\Longleftrightarrow\quad
G\hookrightarrow S\hookrightarrow P,\quad S\text{ simple},\ P\text{ finitely presented}.}
$$

Here $S$ need not be finitely generated or finitely presented. We prove the equivalence using the [Higman embedding theorem](../../../../../higman-s-embedding-theorem.md), [Britton's lemma](../../../../../britton-s-lemma.md) and the [normal form theorem for a free product](../../../../../normal-form-theorem-for-a-free-product.md). The original characterization is Theorem I of [An algebraic characterization of groups with soluble word problem](https://www.cambridge.org/core/journals/journal-of-the-australian-mathematical-society/article/an-algebraic-characterization-of-groups-with-soluble-word-problem1/748FFD937CEA3727E812C8CDB9CC59B9).

First suppose the embeddings exist. Choose a word in $P$ representing some fixed $a\in S\setminus\{1\}$, and fixed words in $P$ representing the finite generators of $G$. Given a word $w$ in those generators, one search enumerates proofs that $w=1$ in the [finite group presentation](../../../../../finite-group-presentation.md) of $P$. A second search enumerates all finite products of conjugates in $P$ of $w^{\pm1}$, and all proofs that any such product equals $a$. All these searches are effective: a proof of equality is a finite product of conjugates of defining relators, checked in the [free group](../../../../../free-group.md), and [dovetailing](../../../../../dovetailing.md) handles the countably many candidates.

If $w\ne1$, simplicity gives $\langle\!\langle w\rangle\!\rangle_S=S$, so $a$ is such a finite product with conjugators in $S$, which are also elements of $P$. The second search eventually succeeds. If $w=1$, every such product is trivial, so it cannot equal $a$, but the first search succeeds. Running the two searches in parallel thus decides the [word problem for a group](../../../../../word-problem-for-groups.md) in $G$. This is [semidecision of nonidentity in simple subgroups](../../../../../semidecision-of-nonidentity-in-simple-subgroups.md); no enumeration of $S$ or word algorithm for $P$ is required. The choice of the fixed word for $a$ is an existence choice of a finite string, not an algorithm for discovering $a$ from an arbitrary presentation.

Conversely suppose the [word problem for a group](../../../../../word-problem-for-groups.md) in $G$ is soluble. We construct a [recursive simple envelope by cyclic HNN extensions](../../../../../recursive-simple-envelope-by-cyclic-hnn-extensions.md), keeping all effectiveness requirements explicit. Start with $P_0=G*\langle a\rangle$, where $a$ has infinite order. Reduced [free product](../../../../../free-product.md) words give a word algorithm for $P_0$ and an algorithm testing membership in $\langle a\rangle$ and recovering its exponent. The original null words of $G$ are decidable and therefore enumerable, so $P_0$ has a [recursive presentation of a group](../../../../../recursive-presentation-of-a-group.md).

Inductively assume $P_n$ has an effectively enumerable generating set, a recursive presentation, a word algorithm, and an algorithm for membership and exponent in $\langle a\rangle$. Form $B_n=P_n*\langle z_n\rangle$. For each nonidentity word $g$ in $P_n$, introduce distinct [stable letters](../../../../../stable-letter.md) $t_{n,g},s_{n,g}$, and introduce another letter $s_{n,0}$, with relations

$$
t_{n,g}^{-1}[g,z_n]t_{n,g}=a,\qquad
s_{n,g}^{-1}(gz_n)s_{n,g}=a,\qquad
s_{n,0}^{-1}z_ns_{n,0}=a.
$$

Let $P_{n+1}$ be this multiple [HNN extension](../../../../../hnn-extension.md) of $B_n$. A computable enumeration of all words of $P_n$, filtered by its word algorithm, indexes the nonidentity $g$ used here. Repeated representatives of the same element cause no difficulty: their stable letters are simply distinct.

Every associated subgroup in these relations is infinite cyclic. For $g\ne1$, the words $gz_n$ and $[g,z_n]$ are cyclically reduced [free product](../../../../../free-product.md) words with respectively two and four syllables; their nonzero $k$th powers have lengths $2|k|$ and $4|k|$. Therefore the reduced syllable length of an input bounds the finitely many possible exponents needed to decide membership in each subgroup and find the exponent. Membership in $\langle z_n\rangle$ is immediate, and membership in $\langle a\rangle$ is inherited from $P_n$. This proves [effective cyclic membership in a free product](../../../../../effective-cyclic-membership-in-a-free-product.md), including the crucial point that the order of $g$ is never needed.

By [Britton's lemma](../../../../../britton-s-lemma.md), $B_n$ embeds in $P_{n+1}$. To solve its word problem, repeatedly find a [pinch in an HNN extension](../../../../../pinch-in-an-hnn-extension.md) using these membership algorithms, transport the known exponent across its defining isomorphism, and remove two stable letters. With no pinch left, a word retaining stable letters is nontrivial and not in the base; otherwise the base word algorithm applies. The same reduction decides whether an input lies in $\langle a\rangle$: if stable letters remain it does not, and if none remain use the base cyclic-membership algorithm. This verifies the inductive effectiveness claims rather than asserting that HNN extensions automatically preserve decidable word problem. Only the finitely many stable letters in the input need inspection.

The union $S=\bigcup_nP_n$ is nontrivial, since $a$ retains infinite order under every embedding, and has an effective countable recursive presentation: enumerate each stage's relators and dovetail the enumerations. We now prove simplicity. Let $D\triangleleft S$ contain $g\ne1$, and take a stage with $g\in P_n$. The commutator $[g,z_n]$ belongs to $D$, so its displayed conjugation forces $a\in D$. Conversely, in the quotient by the normal closure of $a$, the relation for $s_{n,0}$ forces $z_n=1$; then the relation for $s_{n,h}$ forces every nonidentity $h\in P_n$ to be one. Thus the normal closure of $a$ contains each $P_n$. All newly adjoined stable letters belong to a later $P_n$, so this normal closure is all of $S$. Hence $D=S$, proving that $S$ is a [simple group](../../../../../simple-group.md) containing $G$.

Finally apply the explicit [two-generator HNN embedding](../../../../../two-generator-hnn-embedding.md) from Question 3 to an effective countable list of generators of $S$. Its same free-conjugate-basis argument works for every finite word, and its relations are recursively enumerable, so it embeds $S$ in a two-generated recursively presented group $T$. The [Higman embedding theorem](../../../../../higman-s-embedding-theorem.md) embeds $T$ in a [finitely presented group](../../../../../finitely-presented-group.md) $P$. Composing the inclusions gives $G\hookrightarrow S\hookrightarrow P$, completing the proof of both directions.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
